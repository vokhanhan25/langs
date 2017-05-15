
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
- longint: int
- int64: long long
- char: char
- Kiểu số thực: double

## Record
struct HocSinh {
    int tuoi;
    bool gioitinh;
};

# Mảng tĩnh
## Khai báo
- <Kiểu dữ liệu> <Tên biến>[<số phần tử>];
- <Kiểu dữ liệu> <Tên biến>[<số phần tử>] = {<các giá trị của mảng>};

VD:
```
int a[10];
int b[] = {1, 2, 3};
int c[3] = {4, 5, 6};
```

# Khai báo biến
Cú pháp:
- <Kiểu dữ liệu> <Tên biến>,...;
- <Kiểu dữ liệu> <Tên biến> = <Giá trị khởi tạo>,...;

VD:
``` c++
int a;
int b = 1;
int x, y, z;
int e, f = 2;
bool boo = e < f;
int m = n = 100; // 
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
Ví dụ:
```
int add(int a, int b) {
    return a + b;
}
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
