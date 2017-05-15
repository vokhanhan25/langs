
# Cấu trúc chương trình

```
<Nhập thư viện>

<using namespace std;>

<Định nghĩa kiểu dữ liệu>

<Khai báo biến toàn cục>

<Code hàm số, thủ tục>

int main() {
      <Chương trình chính>
      return 0;
}
```


# Gán giá trị
Dùng = thay vì :=

# Khai báo biến
Cú pháp:
- <Kiểu dữ liệu> <Tên biến>,...;
- <Kiểu dữ liệu> <Tên biến> = <Giá trị khởi tạo>,...;

VD:
``` c++
int a; // biến a kiểu int, chưa khởi tạo
int b = 1; // biến b, khởi tạo giá trị = 1
int x, y, z; // biến x, y, z kiểu int
int m = n = 100; // biến m, n kiểu int, đều khởi tạo = 100
int e, f = 2;
int t = 100 + f * m - n; // Khởi tạo giá trị từ biểu thức
```

# Nhập thư viện
# Cú pháp
```
#include <tên thư viện>
```
Ví dụ: 
```
#include <iostream>
#include <math.h>
#include <string>
```
# Các thư viện thường dùng
- Nhập xuất C: stdio.h
- Nhập xuất C++: iostream
- Toán: math.h hoặc cmath
- Chuỗi C++: string
- Chuỗi C: string.h hoặc cstring
- .....

# Kiểu dữ liệu
- boolean: bool
- Số nguyên
    - 8bit: char
    - 32bit: int, long
    - 64bit: long long
    - Các kiểu trên là số nguyên có dấu, muốn chuyển thành không dấu thêm unsigned trước tên kiểu
- Số thực
    - 64bit: double
    - 32bit: float
    - Nên ưu tiên dùng double
- Kí tự: char (char vừa là kí tự vừa là số)
## stdint
Thư viện stdint.h cung cấp tên gọi khác cho các kiểu số nguyên.
Ví dụ:
- uint8_t: số nguyên không dấu 8bit
- int16_t: số nguyên có dấu 16bit

## Kiểu cấu trúc
```
struct HocSinh {
    int tuoi;
    bool gioitinh;
};
```

## Mảng tĩnh
### Khai báo
- <Kiểu dữ liệu> <Tên biến>[<số phần tử>];
- <Kiểu dữ liệu> <Tên biến>[<số phần tử>] = {<các giá trị của mảng>};

VD:
```
int a[10]; // mảng int 10 phần tử
int b[] = {1, 2, 3, 4}; // mảng 4 phần tử, có giá trị lần lượt 1, 2, 3, 4
int c[3] = {4, 5, 6}; // mảng 3 phần tử
```


# Nhập, xuất (màn hình)
## Nhập xuất kiểu C++
``` c++
#include <iostream>
using namespace std;

void main() {
     cout << 100 << 101;
}
```


# Hàm số, thủ tục
## Cú pháp
```
<Kiểu dữ liệu trả về> <Tên hàm>(<danh sách biến truyền vào>) {
      <Code>
      return <giá trị trả về>;
}
```

Nếu hàm không cần trả về thì kiểu dữ liệu là void.
Để truyền tham biến, thêm dấu & sau kiểu dữ liệu.
Ví dụ:

```
int add(int a, int b) {
    return a + b;
}

void swap(int& a, int& b) {
    int t = a;
    a = b;
    b = a;
}
```
