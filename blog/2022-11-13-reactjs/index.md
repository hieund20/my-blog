---
slug: reactjs
title: Change any Value of an Object in an Array
authors: hieudnguyen
tags: [tech, reactjs]
---

Hi, today I will guide you the way to change any value of an `Object` in an `Array` in ReactJS (Hook).
I have five step for you:

1. Clone an `Array`.
2. Find Index of `Object` in `Array`
3. Find Element to change in `Array`
4. Use `splice` method
5. Set new state

```JSX
import React, { useState } from 'react';

const USER_LIST = [
  {
    id: 'f40ebfb0-c716-4ecd-9745-41ee7c73277d',
    name: 'John Doe',
    age: 25,
  },
  {
    id: '5cadc5d2-e175-4eab-8e0c-2197e6357fb1',
    name: 'James Lucas',
    age: 22,
  },
  {
    id: '8c3475e2-dced-46d0-b525-438bfb9662f6',
    name: 'Michael Maguire',
    age: 29,
  },
];

const App = () => {
  const [userList, setUserList] = useState(USER_LIST);

  const onChangeUserName = (id) => {
    //1. Clone Array
    let userListClone = [...userList];
    //2. Find Index of Element in Array
    let index = userListClone.findIndex((element) => element.id === id);
    //3. Find Element to change in Array
    let element = userListClone.find((element) => element.id === id);
    //4. Use splice method
    userListClone.splice(index, 1, {
      ...element,
      name: 'Hieu Nguyen',
    });
    //5. Set new state
    setUserList(userListClone);
  };

  return (
    <div>
      <div>
        {userList.map((item, index) => (
          <div key={index}>
            <span>
              {index} - {item.name} - {item.age}
            </span>
            <button onClick={() => onChangeUserName(item.id)}>Change</button>
          </div>
        ))}
      </div>

      <button onClick={() => setUserList(USER_LIST)}>Reset Change</button>
    </div>
  );
};

export default App;
```

Run demo in [Stackblitz](https://stackblitz.com/edit/react-1htn5e?file=src/App.js)

Thanks for reading !
