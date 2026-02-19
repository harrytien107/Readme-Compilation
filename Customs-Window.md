# Custom Windows

## Mục lục

[Cài Glass Effect cho hệ thống](#glass-effect)

[Cài đặt giảm Ram](#reduce-ram)

[Đổi giao diện chuột phải win 11 thành win 10](#change-right-click)

[Fix lag chuột phải khi bấm](#fix-lag-right-click)

[Xóa icon shortcut trên ứng dụng hiển thị ngoài desktop](#remove-icon-shortcut)

## Glass Effect

Làm đẹp giao diện Windows 11 thành giao diện glass effect

- [Nilesoft Shell](#nilesoft-shell)

- [Windhawk](#windhawk)

- [Chris Titus Tech's Windows Utility](#chris-titus-techs-windows-utility)

### Nilesoft Shell

Tôi chỉ để làm lại css của win 11

- [Download](https://nilesoft.org/)

Dưới đây là một số mods và settings tôi dùng trong Nilesoft Shell:

Thứ nhất bạn vào thư mục cài đặt của Nilesoft Shell, tôi cài mặc định nên là `C:\Program Files\Nilesoft Shell\import` có các file cấu hình. Nếu bạn để thư mục cài đặt ở nơi khác thì bạn vào thư mục đó nhé (Gợi ý có thể dùng [Everything](https://www.voidtools.com/) để tìm thư mục cài đặt).

Vào file `theme.nss` để chỉnh sửa giao diện theo ý muốn hoặc tham khảo [Github](https://github.com/catppuccin/nilesoft-shell/tree/main) này.

[Tham khảo video này](https://youtu.be/HwDcOhlaJsQ?si=5grpj4DzuRdp1NHn)

### Windhawk

- [Download](https://windhawk.net/)

- [Video hướng dẫn](https://www.youtube.com/watch?v=FDAdfMLDzik)

Dưới đây là một số mods và settings tôi dùng trong Windhawk:

Lưu ý: nếu bạn lấy code của tôi thì chỉ cần vào mục `Settings` của mods chọn `Textual mode` rồi dán code vào và save lại. Hoặc có thể vào mục `Advanced` ở trường `Mod settings` dán đoạn json vào và save lại.

1. Translucent Windows

- Settings:

```yaml
RenderingMod:
  ThemeBackground: 1
  SysColors: 1
  AccentColorControls: 1
type: acrylicblur
AccentBlurBehind: '00000000'
FlyoutsEffects: 0
ImmersiveDarkTitle: 1
ExtendFrame: 1
CornerOption: default
RainbowSpeed: 5
TitlebarColor:
  ColorTitlebar: 1
  RainbowTitlebar: 1
  titlerbarstyles_active: f4b8e4
  titlerbarstyles_inactive: f4b8e4
TitlebarTextColor:
  ColorTitlebarText: 0
  RainbowTextColor: 0
  titlerbarcolorstyles_active: f4b8e4
  titlerbarcolorstyles_inactive: f4b8e4
BorderColor:
  ColorBorder: 1
  RainbowBorder: 1
  borderstyles_active: f4b8e4
  borderstyles_inactive: f4b8e4
RuledPrograms:
  - target: WINWORD.EXE
    RenderingMod:
      ThemeBackground: 0
      AccentColorControls: 0
    type: acrylicblur
    AccentBlurBehind: ''
    ImmersiveDarkTitle: 0
    ExtendFrame: 0
    CornerOption: ''
    RainbowSpeed: 5
    TitlebarColor:
      ColorTitlebar: 0
      RainbowTitlebar: 0
      titlerbarstyles_active: ''
      titlerbarstyles_inactive: ''
    TitlebarTextColor:
      ColorTitlebarText: 0
      RainbowTextColor: 0
      titlerbarcolorstyles_active: ''
      titlerbarcolorstyles_inactive: ''
    BorderColor:
      ColorBorder: 1
      RainbowBorder: 1
      borderstyles_active: f4b8e4
      borderstyles_inactive: f4b8e4
  - target: EXCEL.EXE
    RenderingMod:
      ThemeBackground: 0
      AccentColorControls: 0
    type: acrylicblur
    AccentBlurBehind: ''
    ImmersiveDarkTitle: 0
    ExtendFrame: 0
    CornerOption: ''
    RainbowSpeed: 5
    TitlebarColor:
      ColorTitlebar: 0
      RainbowTitlebar: 0
      titlerbarstyles_active: ''
      titlerbarstyles_inactive: ''
    TitlebarTextColor:
      ColorTitlebarText: 0
      RainbowTextColor: 0
      titlerbarcolorstyles_active: ''
      titlerbarcolorstyles_inactive: ''
    BorderColor:
      ColorBorder: 1
      RainbowBorder: 1
      borderstyles_active: f4b8e4
      borderstyles_inactive: f4b8e4
  - target: POWERPNT.EXE
    RenderingMod:
      ThemeBackground: 0
      AccentColorControls: 0
    type: acrylicblur
    AccentBlurBehind: ''
    ImmersiveDarkTitle: 0
    ExtendFrame: 0
    CornerOption: ''
    RainbowSpeed: 5
    TitlebarColor:
      ColorTitlebar: 0
      RainbowTitlebar: 0
      titlerbarstyles_active: ''
      titlerbarstyles_inactive: ''
    TitlebarTextColor:
      ColorTitlebarText: 0
      RainbowTextColor: 0
      titlerbarcolorstyles_active: ''
      titlerbarcolorstyles_inactive: ''
    BorderColor:
      ColorBorder: 1
      RainbowBorder: 1
      borderstyles_active: f4b8e4
      borderstyles_inactive: f4b8e4
```

- Advanced:

```json
{
    "RenderingMod.ThemeBackground": 1,
    "RenderingMod.SysColors": 1,
    "RenderingMod.AccentColorControls": 1,
    "type": "acrylicblur",
    "AccentBlurBehind": "00000000",
    "FlyoutsEffects": 0,
    "ImmersiveDarkTitle": 1,
    "ExtendFrame": 1,
    "CornerOption": "default",
    "RainbowSpeed": 5,
    "TitlebarColor.ColorTitlebar": 1,
    "TitlebarColor.RainbowTitlebar": 1,
    "TitlebarColor.titlerbarstyles_active": "f4b8e4",
    "TitlebarColor.titlerbarstyles_inactive": "f4b8e4",
    "TitlebarTextColor.ColorTitlebarText": 0,
    "TitlebarTextColor.RainbowTextColor": 0,
    "TitlebarTextColor.titlerbarcolorstyles_active": "f4b8e4",
    "TitlebarTextColor.titlerbarcolorstyles_inactive": "f4b8e4",
    "BorderColor.ColorBorder": 1,
    "BorderColor.RainbowBorder": 1,
    "BorderColor.borderstyles_active": "f4b8e4",
    "BorderColor.borderstyles_inactive": "f4b8e4",
    "RuledPrograms[0].target": "WINWORD.EXE",
    "RuledPrograms[0].RenderingMod.ThemeBackground": 0,
    "RuledPrograms[0].RenderingMod.AccentColorControls": 0,
    "RuledPrograms[0].type": "acrylicblur",
    "RuledPrograms[0].AccentBlurBehind": "",
    "RuledPrograms[0].ImmersiveDarkTitle": 0,
    "RuledPrograms[0].ExtendFrame": 0,
    "RuledPrograms[0].CornerOption": "",
    "RuledPrograms[0].RainbowSpeed": 5,
    "RuledPrograms[0].TitlebarColor.ColorTitlebar": 0,
    "RuledPrograms[0].TitlebarColor.RainbowTitlebar": 0,
    "RuledPrograms[0].TitlebarColor.titlerbarstyles_active": "",
    "RuledPrograms[0].TitlebarColor.titlerbarstyles_inactive": "",
    "RuledPrograms[0].TitlebarTextColor.ColorTitlebarText": 0,
    "RuledPrograms[0].TitlebarTextColor.RainbowTextColor": 0,
    "RuledPrograms[0].TitlebarTextColor.titlerbarcolorstyles_active": "",
    "RuledPrograms[0].TitlebarTextColor.titlerbarcolorstyles_inactive": "",
    "RuledPrograms[0].BorderColor.ColorBorder": 1,
    "RuledPrograms[0].BorderColor.RainbowBorder": 1,
    "RuledPrograms[0].BorderColor.borderstyles_active": "f4b8e4",
    "RuledPrograms[0].BorderColor.borderstyles_inactive": "f4b8e4",
    "RuledPrograms[1].target": "EXCEL.EXE",
    "RuledPrograms[1].RenderingMod.ThemeBackground": 0,
    "RuledPrograms[1].RenderingMod.AccentColorControls": 0,
    "RuledPrograms[1].type": "acrylicblur",
    "RuledPrograms[1].AccentBlurBehind": "",
    "RuledPrograms[1].ImmersiveDarkTitle": 0,
    "RuledPrograms[1].ExtendFrame": 0,
    "RuledPrograms[1].CornerOption": "",
    "RuledPrograms[1].RainbowSpeed": 5,
    "RuledPrograms[1].TitlebarColor.ColorTitlebar": 0,
    "RuledPrograms[1].TitlebarColor.RainbowTitlebar": 0,
    "RuledPrograms[1].TitlebarColor.titlerbarstyles_active": "",
    "RuledPrograms[1].TitlebarColor.titlerbarstyles_inactive": "",
    "RuledPrograms[1].TitlebarTextColor.ColorTitlebarText": 0,
    "RuledPrograms[1].TitlebarTextColor.RainbowTextColor": 0,
    "RuledPrograms[1].TitlebarTextColor.titlerbarcolorstyles_active": "",
    "RuledPrograms[1].TitlebarTextColor.titlerbarcolorstyles_inactive": "",
    "RuledPrograms[1].BorderColor.ColorBorder": 1,
    "RuledPrograms[1].BorderColor.RainbowBorder": 1,
    "RuledPrograms[1].BorderColor.borderstyles_active": "f4b8e4",
    "RuledPrograms[1].BorderColor.borderstyles_inactive": "f4b8e4",
    "RuledPrograms[2].target": "POWERPNT.EXE",
    "RuledPrograms[2].RenderingMod.ThemeBackground": 0,
    "RuledPrograms[2].RenderingMod.AccentColorControls": 0,
    "RuledPrograms[2].type": "acrylicblur",
    "RuledPrograms[2].AccentBlurBehind": "",
    "RuledPrograms[2].ImmersiveDarkTitle": 0,
    "RuledPrograms[2].ExtendFrame": 0,
    "RuledPrograms[2].CornerOption": "",
    "RuledPrograms[2].RainbowSpeed": 5,
    "RuledPrograms[2].TitlebarColor.ColorTitlebar": 0,
    "RuledPrograms[2].TitlebarColor.RainbowTitlebar": 0,
    "RuledPrograms[2].TitlebarColor.titlerbarstyles_active": "",
    "RuledPrograms[2].TitlebarColor.titlerbarstyles_inactive": "",
    "RuledPrograms[2].TitlebarTextColor.ColorTitlebarText": 0,
    "RuledPrograms[2].TitlebarTextColor.RainbowTextColor": 0,
    "RuledPrograms[2].TitlebarTextColor.titlerbarcolorstyles_active": "",
    "RuledPrograms[2].TitlebarTextColor.titlerbarcolorstyles_inactive": "",
    "RuledPrograms[2].BorderColor.ColorBorder": 1,
    "RuledPrograms[2].BorderColor.RainbowBorder": 1,
    "RuledPrograms[2].BorderColor.borderstyles_active": "f4b8e4",
    "RuledPrograms[2].BorderColor.borderstyles_inactive": "f4b8e4"
}
```

2. Windows 11 Notification Center Styler

- Settings:

```yaml
theme: WindowGlass_variant_alternative
controlStyles:
  - target: ''
    styles:
      - ''
styleConstants:
  - ''
themeResourceVariables:
  - ''
```

- Advanced:

```json
{
    "theme":"WindowGlass_variant_alternative",
    "controlStyles[0].target":"",
    "controlStyles[0].styles[0]":"",
    "styleConstants[0]":"",
    "themeResourceVariables[0]":""
}
```

3. Windows 11 Start Menu Styler

- Settings:

```yaml
theme: TranslucentStartMenu
disableNewStartMenuLayout: 1
controlStyles:
  - target: ''
    styles:
      - ''
webContentStyles:
  - target: ''
    styles:
      - ''
webContentCustomJs: ''
styleConstants:
  - ''
resourceVariables:
  - variableKey: ''
    value: ''
```

- Advanced:

```json
{
    "theme":"TranslucentStartMenu",
    "disableNewStartMenuLayout":1,
    "controlStyles[0].target":"",
    "controlStyles[0].styles[0]":"",
    "webContentStyles[0].target":"",
    "webContentStyles[0].styles[0]":"",
    "webContentCustomJs":"",
    "styleConstants[0]":"",
    "resourceVariables[0].variableKey":"",
    "resourceVariables[0].value":""
}
```

4. Windows 11 Taskbar Styler

- Settings:

```yaml
theme: ''
controlStyles:
  - target: Taskbar.TaskbarFrame > Grid#RootGrid > Taskbar.TaskbarBackground > Grid > Rectangle#BackgroundFill
    styles:
      - Fill=$CommonBgBrush
  - target: Taskbar.TaskbarBackground#HoverFlyoutBackgroundControl > Grid > Rectangle#BackgroundFill
    styles:
      - Fill=$CommonBgBrush
  - target: Rectangle#BackgroundStroke
    styles:
      - Visibility=Collapsed
  - target: MenuFlyoutPresenter > Border
    styles:
      - Background=$CommonBgBrush
      - BorderThickness=0,0,0,0
      - CornerRadius=14
      - Padding=3,4,3,4
  - target: Border#OverflowFlyoutBackgroundBorder
    styles:
      - Background=$CommonBgBrush
      - BorderThickness=0,0,0,0
      - CornerRadius=15
      - Margin=-2,-2,-2,-2
  - target: Grid#ConfirmatorMainGrid
    styles:
      - Background=$CommonBgBrush
      - BorderThickness=0
  - target: WindowsInternal.ComposableShell.Experiences.TextInput.Common.InputSwitcher > ContentControl > ContentPresenter > Grid
    styles:
      - Background=Transparent
      - BorderThickness=0
  - target: WindowsInternal.ComposableShell.Experiences.TextInput.Common.InputSwitcher > ContentControl > ContentPresenter > Grid > Grid
    styles:
      - Background=Transparent
styleConstants:
  - CommonBgBrush=Transparent
resourceVariables:
  - variableKey: ''
    value: ''
```

- Advanced:

```json
{
    "controlStyles[0].target":"Taskbar.TaskbarFrame > Grid#RootGrid > Taskbar.TaskbarBackground > Grid > Rectangle#BackgroundFill",
    "controlStyles[0].styles[0]":"Fill=$CommonBgBrush",
    "controlStyles[1].target":"Taskbar.TaskbarBackground#HoverFlyoutBackgroundControl > Grid > Rectangle#BackgroundFill",
    "controlStyles[1].styles[0]":"Fill=$CommonBgBrush",
    "controlStyles[2].target":"Rectangle#BackgroundStroke",
    "controlStyles[2].styles[0]":"Visibility=Collapsed",
    "controlStyles[3].target":"MenuFlyoutPresenter > Border",
    "controlStyles[3].styles[0]":"Background=$CommonBgBrush",
    "controlStyles[3].styles[1]":"BorderThickness=0,0,0,0",
    "controlStyles[3].styles[2]":"CornerRadius=14",
    "controlStyles[3].styles[3]":"Padding=3,4,3,4",
    "controlStyles[4].target":"Border#OverflowFlyoutBackgroundBorder",
    "controlStyles[4].styles[0]":"Background=$CommonBgBrush",
    "controlStyles[4].styles[1]":"BorderThickness=0,0,0,0",
    "controlStyles[4].styles[2]":"CornerRadius=15",
    "controlStyles[4].styles[3]":"Margin=-2,-2,-2,-2",
    "controlStyles[5].target":"Grid#ConfirmatorMainGrid",
    "controlStyles[5].styles[0]":"Background=$CommonBgBrush",
    "controlStyles[5].styles[1]":"BorderThickness=0",
    "controlStyles[6].target":"WindowsInternal.ComposableShell.Experiences.TextInput.Common.InputSwitcher > ContentControl > ContentPresenter > Grid",
    "controlStyles[6].styles[0]":"Background=Transparent",
    "controlStyles[6].styles[1]":"BorderThickness=0",
    "controlStyles[7].target":"WindowsInternal.ComposableShell.Experiences.TextInput.Common.InputSwitcher > ContentControl > ContentPresenter > Grid > Grid",
    "controlStyles[7].styles[0]":"Background=Transparent",
    "styleConstants[0]":"CommonBgBrush=Transparent"
}
```

### Chris Titus Tech's Windows Utility

Đây là một Interface terminal rất hữu ích của Chris Titus Tech. Ông ấy đã tóm tắt các lệnh hữu ích thành các button.

- [Download](https://github.com/ChrisTitusTech/winutil)

- [Video hướng dẫn](https://www.youtube.com/watch?v=6UQZ5oQg8XA)

## Reduce Ram

Giảm lượng ram sử dụng [Mem Reduct](https://memreduct.org/)

## Change right click

Chuyển giao diện chuột phải từ win 11 thành win 10

**Cách 1:** Mở PowerShell với quyền Admin

```bash
irm christitus.com/win | iex
```

**Cách 2:** Mở command prompt với quyền admin

```bash
reg.exe add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f /ve
```

Sau khi chuyển về win 10, mà bạn muốn có css của win 11 thì tải `Nilesoft Shell` hoặc `Windhawk`.

## Fix lag right click

Fix độ trễ khi bấm chuột phải

**Cách 1:** Mở Command Prompt với quyền Admin.

```bash
reg add HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2} /f
```

**Cách 2:** Registry Editor

Copy đường dẫn dưới đây và paste vào Registry Editor:

```bash
Computer\HKEY_CURRENT_USER\Control Panel\Desktop
```

Tìm `Menu Show Delay` đổi `value` từ `400` thành `0` (hoặc bằng số nào tùy thích càng nhỏ càng tốt).

## Remove icon shortcut

Xóa icon shortcut khi hiển thị ngoài desktop

B1: Mở `registry editor`

B2: Copy đường dẫn dưới đây và paste vào Registry Editor:

```bash
Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\
```
B3: Nhấn chuột phải vào `Explorer` chọn `New` -> `Key` và đặt tên là `Shell Icons`

B4: Nhấn chuột phải vào `Shell Icons` chọn `New` -> `String Value` và đặt tên là `29`

B5: Double click vào `29` điền vào `Value data`:

```bash
%windir%\System32\shell32.dll,-50
```

B6: Restart

Có thể restart `explorer` bằng cách vào `Task Manager` chọn `explorer` và nhấn `restart`.

Hoặc có thể gõ lệnh sau:

```bash
taskkill /f /im explorer.exe & start explorer.exe
```

Hoặc restart máy.

[Video hướng dẫn](https://youtu.be/TFQ42fCVT_w?si=xvxjhoy2Bfk5nCth)