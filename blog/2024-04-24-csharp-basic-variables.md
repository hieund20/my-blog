---
slug: csharp-basic-variables
title: Biến và kiểu dữ liệu trong C#
authors: ndhieu
tags: [.NET Framework][C#]
---

## Biến trong C#
Trong C#, biến là một khối dữ liệu có thể thay đổi giá trị trong quá trình thực thi của chương trình. Mỗi biến trong C# đều có một kiểu dữ liệu và một tên duy nhất để xác định nó. Dưới đây là một số điểm cơ bản về biến trong C#


<b>Khai báo biến</b>: Để khai báo một biến trong C#, bạn sử dụng cú pháp sau:
```cs
<kiểu_dữ_liệu> <tên_biến>;
```

Ví dụ:
```cs
int age;
string name;
```

<b>Gán giá trị cho biến</b>: Bạn có thể gán giá trị cho biến khi khai báo hoặc sau đó trong chương trình:

```cs
int age = 30;
string name = "John";
```


<b>Thay đổi giá trị của biến</b>: Bạn có thể thay đổi giá trị của một biến bằng cách gán một giá trị mới cho nó:

```cs
age = 35;
```

<b>Biến cục bộ và biến toàn cục</b>: Biến cục bộ được khai báo trong phạm vi của một phương thức hoặc một khối mã cụ thể. Biến toàn cục được khai báo bên ngoài mọi phương thức và có thể truy cập từ bất kỳ đâu trong chương trình.


<b>Hằng số (constant)</b>: Hằng số là một loại biến có giá trị không thể thay đổi sau khi đã được gán giá trị ban đầu. Để định nghĩa một hằng số trong C#, bạn sử dụng từ khóa const.
```cs
const double Pi = 3.14;
```

## Kiểu dữ liệu trong C#
Trong C#, có nhiều loại kiểu dữ liệu khác nhau được sử dụng để định nghĩa các biến hoặc hằng số, mỗi kiểu dữ liệu có đặc điểm và phạm vi sử dụng riêng. Dưới đây là một số kiểu dữ liệu phổ biến trong C#.


<b>Kiểu số nguyên (Integer Types):</b>
- `int`: Kiểu số nguyên có kích thước 32 bit, có thể lưu trữ giá trị từ -2,147,483,648 đến 2,147,483,647
- `long`: Kiểu số nguyên có kích thước 64 bit, có thể lưu trữ giá trị từ -9,223,372,036,854,775,808 đến 9,223,372,036,854,775,807.
- `short`: Kiểu số nguyên có kích thước 16 bit, có thể lưu trữ giá trị từ -32,768 đến 32,767.
- `byte`: Kiểu số nguyên không dấu có kích thước 8 bit, có thể lưu trữ giá trị từ 0 đến 255.


<b>Kiểu số thực (Floating-Point Types):</b>
- `float`: Kiểu số thực dấu chấm động có kích thước 32 bit, có độ chính xác khoảng 6-9 chữ số thập phân.
- `double`: Kiểu số thực dấu chấm động có kích thước 64 bit, có độ chính xác cao hơn float.


<b>Kiểu ký tự (Character Type):</b>
- `char`: Kiểu ký tự Unicode có kích thước 16 bit, được sử dụng để lưu trữ một ký tự Unicode.


<b>Kiểu chuỗi (String Type):</b>
- `string`: Kiểu dữ liệu chuỗi, sử dụng để lưu trữ một chuỗi các ký tự Unicode.


<b>Kiểu Boolean (Boolean Type):</b>
`bool`: Kiểu dữ liệu boolean, chỉ có thể lưu trữ hai giá trị là true hoặc false.


<b>Kiểu hằng số (Constant Type):</b>
`const`: Kiểu hằng số được sử dụng để định nghĩa các biến có giá trị không thay đổi trong suốt vòng đời của chương trình.


Ngoài ra, C# cũng hỗ trợ kiểu dữ liệu `decimal` để lưu trữ các số thập phân có độ chính xác cố định, kiểu dữ liệu `object` cho các đối tượng không xác định trước, và kiểu dữ liệu `dynamic` cho biến có thể thay đổi kiểu dữ liệu trong quá trình thực thi.


