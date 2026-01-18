# Cài đặt môi trường Msys2

Cài msys2 để setup môi trường C/C++ hoặc Python trên _local_ (trên windows)

## 1. Cài đặt Msys2

Bước 1: Truy cập trang chủ của Msys2

- Truy cập trang chủ của Msys2: [https://www.msys2.org/](https://www.msys2.org/)
- Tải về phiên bản phù hợp với hệ điều hành của bạn
- Cài đặt theo hướng dẫn trên trang chủ

Bước 2: Double click vào file .exe vừa tải về

Bước 3: Nhập thư mục cài đặt bạn muốn sử dụng. Chúng tôi khuyên bạn nên sử dụng thư mục mặc định, xem hướng dẫn về thư mục cài đặt để biết thêm thông tin.

<img alt="image" src="./pic/setup-enviroment-msys2/install-2-path-dark.png" width="800">

Bước 4: Khi hoàn tất, hãy nhấp vào nút Hoàn tất.

<img alt="image" src="./pic/setup-enviroment-msys2/install-3-finish-dark.png" width="800">

Bước 5: Giờ đây MSYS2 đã sẵn sàng và một cửa sổ dòng lệnh cho môi trường UCRT64 sẽ được khởi chạy.

<img alt="image" src="./pic/setup-enviroment-msys2/install-4-terminal-dark.png" width="800">

Bước 6: Có thể bạn sẽ cần cài đặt một số công cụ như mingw-w64 GCC để bắt đầu biên dịch dự án. Chạy lệnh sau:

Binary Packages:

- ucrt64

```bash
pacman -S mingw-w64-ucrt-x86_64-gcc
```

- mingw64

```bash
pacman -S mingw-w64-x86_64-gcc
```

- mingw32

```bash
pacman -S mingw-w64-i686-gcc
```

Bước 7: Cửa sổ terminal sẽ hiển thị kết quả như bên dưới. Nhấn 'Enter' để tiếp tục:

```bash
resolving dependencies...
looking for conflicting packages...

Packages (15) mingw-w64-ucrt-x86_64-binutils-2.41-2
            mingw-w64-ucrt-x86_64-crt-git-11.0.0.r216.gffe883434-1
            mingw-w64-ucrt-x86_64-gcc-libs-13.2.0-2  mingw-w64-ucrt-x86_64-gmp-6.3.0-2
            mingw-w64-ucrt-x86_64-headers-git-11.0.0.r216.gffe883434-1
            mingw-w64-ucrt-x86_64-isl-0.26-1  mingw-w64-ucrt-x86_64-libiconv-1.17-3
            mingw-w64-ucrt-x86_64-libwinpthread-git-11.0.0.r216.gffe883434-1
            mingw-w64-ucrt-x86_64-mpc-1.3.1-2  mingw-w64-ucrt-x86_64-mpfr-4.2.1-2
            mingw-w64-ucrt-x86_64-windows-default-manifest-6.4-4
            mingw-w64-ucrt-x86_64-winpthreads-git-11.0.0.r216.gffe883434-1
            mingw-w64-ucrt-x86_64-zlib-1.3-1  mingw-w64-ucrt-x86_64-zstd-1.5.5-1
            mingw-w64-ucrt-x86_64-gcc-13.2.0-2

Total Download Size:    49.38 MiB
Total Installed Size:  418.82 MiB

:: Proceed with installation? [Y/n]
[... downloading and installation continues ...]
```

Bước 8: Giờ đây bạn có thể gọi gcc để biên dịch phần mềm cho Windows.

```bash
$ gcc --version
```

Bước 9: Sau khi cài đặt MSYS2, hệ thống sẽ tự động cập nhật thông qua pacman, [xem hướng dẫn cập nhật để biết thêm thông tin](https://www.msys2.org/docs/updating/).

Bước 10: Thiết lập môi trường vào máy tính vào vị trí thư mục ở `bước 3` copy đường dẫn đến thư mục đó và thêm vào biến môi trường `Path`.

Bước 11: Tìm kiếm `env` trong `start menu` và chọn `Edit the system environment variables`.

Bước 12: Nhấp vào nút `Environment Variables...`.

Bước 13: Trong cửa sổ `Environment Variables`, tìm đến mục `System variables` và chọn `Path`. Sau đó nhấp vào nút `Edit...`.

Bước 14: Nhấp vào nút `New` và thêm đường dẫn đến thư mục MSYS2 vào.

Ví dụ trong máy `Glass`
```path
D:\Enviroment\msys2\mingw64\bin
```

Bước 15: Nhấp vào nút `OK` để đóng cửa sổ `Environment Variables`.

## 2. Sự khác biệt giữa các gói (Environment)

Trong môi trường MSYS2, sự khác biệt chính nằm ở **Thư viện C Runtime (CRT)** và **Kiến trúc CPU**:

1. **UCRT64** (`mingw-w64-ucrt-x86_64-...`)
   - **Kiến trúc:** 64-bit.
   - **Runtime:** **UCRT** (Universal C Runtime) - Chuẩn mới của Windows 10/11.
   - **Đặc điểm:** Tương thích tốt hơn với chuẩn C/C++ hiện đại và MSVC.
   - **Khuyên dùng:** ✅ **Nên dùng cho hầu hết dự án mới.**

2. **MINGW64** (`mingw-w64-x86_64-...`)
   - **Kiến trúc:** 64-bit.
   - **Runtime:** **MSVCRT** (Cũ).
   - **Đặc điểm:** Tương thích ngược tốt với Windows cũ (Win 7).
   - **Khuyên dùng:** Chỉ dùng khi cần hỗ trợ hệ thống cũ.

3. **MINGW32** (`mingw-w64-i686-...`)
   - **Kiến trúc:** 32-bit.
   - **Khuyên dùng:** ❌ Chỉ dùng khi cần build ứng dụng 32-bit.

| Môi trường  | Package Prefix | Kiến trúc | Runtime     | Mục đích                    |
| :---------- | :------------- | :-------- | :---------- | :-------------------------- |
| **UCRT64**  | `ucrt-x86_64`  | 64-bit    | UCRT (Mới)  | ✅ **Mặc định / Dự án mới** |
| **MINGW64** | `x86_64`       | 64-bit    | MSVCRT (Cũ) | Tương thích Windows cũ      |
| **MINGW32** | `i686`         | 32-bit    | MSVCRT (Cũ) | Legacy 32-bit               |

## 3. Cài đặt thư viện

Bạn có thể vào đường dẫn này [https://packages.msys2.org/queue](https://packages.msys2.org/queue) để tìm kiếm thư viện bạn cần cài đặt. Ví dụ, nếu bạn cần cài đặt thư viện `SDL2`, bạn có thể tìm kiếm `SDL2` và chọn gói phù hợp với môi trường của bạn. Sau đó, bạn có thể cài đặt thư viện bằng lệnh `pacman -S <package-name>`.

```bash
pacman -S mingw-w64-ucrt-x86_64-SDL2
```
