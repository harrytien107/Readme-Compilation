# Hướng dẫn cài Windows 11 và Office 365

## Mục lục

- [Chuẩn bị usb cứu hộ](./Setup-Window.md#chuẩn-bị-usb-cứu-hộp)

- [Cài Windows 11](./Setup-Window.md#cai-windows-11)

- [Cài Office 365](./Setup-Window.md#cai-office-365)

- [Một số cài đặt tối ưu và làm đẹp windows](./Setup-Window.md#mot-so-cai-tao-toi-uu-va-lam-dep-windows)

## Chuẩn bị usb cứu hộ

Bạn có thể làm theo video hướng dẫn dưới đây [Link video](https://youtu.be/g2tDjh7v-Ok?si=PSa-RFeuJ0qHI6oA)

## Cài Windows 11

Trước tiên bạn phải chuẩn bị một [USB cứu hộ](./Setup-Window.md#chuẩn-bị-usb-cứu-hộp) trước khi cài vì các hướng dẫn sau đây đều liên quan đến đó.

**B1:** Chia ổ đĩa (ít nhất 2 ổ C và D)

**B2:** Lên [Microsoft](https://www.microsoft.com/en-us/software-download/windows11) để tải file windows 11 .iso (lưu ý để vào ổ D, không được phép để vào ổ C)

**B3:** Làm ra file .xml _(nếu muốn windows được cài nhẹ, còn không khỏi tạo cũng được)_

- Cách 1: lên web này tạo [Link](https://schneegans.de/windows/unattend-generator/)

- Cách 2: tải file .xml có sẵn trên github [Link](https://github.com/memstechtips/UnattendedWinstall/blob/main/autounattend.xml#L10)

**B4:** Cắm usb cứu hộ sao đó restart máy, trong lúc đang restart bấm các nút hàng F, để chọn môi trường trong usb cứu hộ

**B5:** Coi theo video cài windows của "Neyako Phạm" [Link](https://vt.tiktok.com/ZS9JhErjobKJd-0MDv3/)

**B6:** Cài lại các phần mềm, sau khi cài lại windows

Mở powershell với quyền admin

```bash
irm christitus.com/win | iex
```

_Lưu ý:_ Do 1 số phần mềm cần cài nằm trên Microsoft Store, mà gần đây nó hay bị lỗi.

> Sửa lỗi Microsoft Store khi bị lỗi Code: 0x80244022

Mở PowerShell với quyền Admin

```bash
Get-AppxPackage -AllUsers *WindowsStore* | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register "$($_.InstallLocation)\AppXManifest.xml"}
```

**B7:** Đi kiếm chỗ cài đặt driver bị thiếu (VD: với máy Lenovo thì cài Lenovo Vantage, vô phần system update)

**B8:** Cài phần mềm Winhance, để tắt/bật windows update

**B9:** Active windows và Microsoft Office

Mở PowerShell với quyền Admin

```bash
irm https://get.activated.win | iex
```

Mở Command Prompt với quyền Admin

```bash
irm https://get.activated.win
```

## Cài Office 365

[Cài Office 365](https://youtu.be/KqKAm97Baeo?si=ig1xETd2GR1MipYM)

[Active Office 365](https://youtu.be/ogfi_py7n8k?si=4Ypv36wrnuGRI-a_)

## Một số cài đặt tối ưu và làm đẹp windows

### Cài Glass Effect cho hệ thống

- [Nilesoft Shell](https://nilesoft.org/)

- [Windhawk](https://windhawk.net/): [Video hướng dẫn](https://www.youtube.com/watch?v=FDAdfMLDzik)

- [Video hướng dẫn dùng của christitus](https://youtu.be/6UQZ5oQg8XA?si=uS8CADOAeooVl9mg)

### Cài đặt giảm Ram:

[Mem Reduct](https://memreduct.org/)

### Đổi giao diện chuột phải win 11 thành win 10

**Cách 1:** Mở PowerShell với quyền Admin

```bash
irm christitus.com/win | iex
```

**Cách 2:** Mở command prompt với quyền admin

```bash
reg add HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2} /f
```

### Fix lag chuột phải khi bấm

**Cách 1:** Mở Command Prompt với quyền Admin.

```bash
reg add HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2} /f
```

**Cách 2:** Registry Editor

Copy đường dẫn dưới đây và paste vào Registry Editor:

```bash
Computer\HKEY_CURRENT_USER\Control Panel\Desktop
```

Tìm `Menu Show Delay` đổi `value` từ `400` thành `0` (hoặc bằng số nào tùy thích càng nhỏ càng tốt)