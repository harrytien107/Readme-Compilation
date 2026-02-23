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

Cho phép hiển thị hiệu ứng mờ tự nhiên trong Windows 11.

- 1. Cấu hình 1:

  Loại trừ các `app bị lỗi giao diện` trong code để vẫn có `viền màu random`!

  - Settings:

    <details>
    <summary>Click to expand</summary>

    ```yaml
    RenderingMod:
      ThemeBackground: 1
      SysColors: 1
      AccentColorControls: 1
    type: acrylicblur
    AccentBlurBehind: 8C000000
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
        type: none
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
        type: none
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
        type: none
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
      - target: mathtype.exe
        RenderingMod:
          ThemeBackground: 0
          AccentColorControls: 0
        type: none
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

    </details>

  - Advanced:

    <details>
    <summary>Click to expand</summary>

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

    </details>

- 2. Cấu hình 2:

  Loại trừ các `app bị lỗi giao diện` bằng `Custom process exclusion list` trong `Advanced`!

  - Settings:

    <details>
    <summary>Click to expand</summary>

    ```yaml
    RenderingMod:
      ThemeBackground: 1
      SysColors: 0
      AccentColorControls: 0
    type: acrylicblur
    AccentBlurBehind: 8C000000
    FlyoutsEffects: 0
    ImmersiveDarkTitle: 0
    ExtendFrame: 1
    CornerOption: default
    RainbowSpeed: 5
    TitlebarColor:
      ColorTitlebar: 1
      RainbowTitlebar: 1
      titlerbarstyles_active: f4b8e4
      titlerbarstyles_inactive: f4b8e4
    TitlebarTextColor:
      ColorTitlebarText: 1
      RainbowTextColor: 1
      titlerbarcolorstyles_active: f4b8e4
      titlerbarcolorstyles_inactive: f4b8e4
    BorderColor:
      ColorBorder: 1
      RainbowBorder: 1
      borderstyles_active: f4b8e4
      borderstyles_inactive: f4b8e4
    RuledPrograms:
      - target: ''
        RenderingMod:
          ThemeBackground: 0
          AccentColorControls: 0
        type: ''
        AccentBlurBehind: ''
        ImmersiveDarkTitle: 0
        ExtendFrame: 0
        CornerOption: ''
        RainbowSpeed: 0
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
          ColorBorder: 0
          RainbowBorder: 0
          borderstyles_active: ''
          borderstyles_inactive: ''
    ```

    </details>

  - Advanced:

    - Mod settings:
      <details>
      <summary>Click to expand</summary>

      ```json
      {
          "RenderingMod.ThemeBackground": 1,
          "RenderingMod.SysColors": 0,
          "RenderingMod.AccentColorControls": 0,
          "type": "acrylicblur",
          "AccentBlurBehind": "8C000000",
          "FlyoutsEffects": 0,
          "ImmersiveDarkTitle": 0,
          "ExtendFrame": 1,
          "CornerOption": "default",
          "RainbowSpeed": 5,
          "TitlebarColor.ColorTitlebar": 1,
          "TitlebarColor.RainbowTitlebar": 1,
          "TitlebarColor.titlerbarstyles_active": "f4b8e4",
          "TitlebarColor.titlerbarstyles_inactive": "f4b8e4",
          "TitlebarTextColor.ColorTitlebarText": 1,
          "TitlebarTextColor.RainbowTextColor": 1,
          "TitlebarTextColor.titlerbarcolorstyles_active": "f4b8e4",
          "TitlebarTextColor.titlerbarcolorstyles_inactive": "f4b8e4",
          "BorderColor.ColorBorder": 1,
          "BorderColor.RainbowBorder": 1,
          "BorderColor.borderstyles_active": "f4b8e4",
          "BorderColor.borderstyles_inactive": "f4b8e4"
      }
      ```

      </details>

    - Custom process exclusion list:
      <details>
      <summary>Click to expand</summary>

      ```
        PDFXEdit.exe
        WINWORD.EXE
        EXCEL.EXE
        POWERPNT.EXE
        mathtype.exe
        UniKeyNT.exe
      ```
      </details>

2. Windows 11 Notification Center Styler

Tùy chỉnh Trung tâm Thông báo và Trung tâm Hành động bằng các chủ đề do người khác đóng góp hoặc tạo chủ đề của riêng bạn.

- Settings:

  <details>
  <summary>Click to expand</summary>

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

  </details>

- Advanced:

  <details>
  <summary>Click to expand</summary>

  ```json
  {
      "theme":"WindowGlass_variant_alternative",
      "controlStyles[0].target":"",
      "controlStyles[0].styles[0]":"",
      "styleConstants[0]":"",
      "themeResourceVariables[0]":""
  }
  ```

  </details>

3. Windows 11 Start Menu Styler

Tùy chỉnh menu Start với các chủ đề do người khác đóng góp hoặc tạo chủ đề của riêng bạn.

- Settings:

  <details>
  <summary>Click to expand</summary>

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

  </details>

- Advanced:

  <details>
  <summary>Click to expand</summary>

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

  </details>

4. Windows 11 Taskbar Styler

Tùy chỉnh thanh tác vụ với các chủ đề do người khác đóng góp hoặc tạo chủ đề của riêng bạn.

- 1. TranslucentTaskbar

  - Settings:

    <details>
    <summary>Click to expand</summary>

    ```yaml
    theme: TranslucentTaskbar
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

    </details>

  - Advanced:

    <details>
    <summary>Click to expand</summary>

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

    </details>

- 2. WindowGlass

  - Settings:

    <details>
    <summary>Click to expand</summary>

    ```yaml
    theme: WindowGlass
    controlStyles:
      - target: Taskbar.TaskbarFrame#TaskbarFrame
        styles:
          - MaxWidth:=900
          - HorizontalAlignment=Auto
          - Width=Auto
          - MinWidth:=500
      - target: Taskbar.TaskbarFrame#TaskbarFrame > Grid#RootGrid
        styles:
          - Margin=30,0,30,5
          - BorderThickness=$BorderThickness
          - BorderBrush:=$BorderBrush
          - CornerRadius=$CornerRadius
          - Background:=Transparent
      - target: Rectangle#BackgroundFill
        styles:
          - Visibility=Visible
          - Fill:=$Background
      - target: Rectangle#BackgroundStroke
        styles:
          - Visibility=Collapsed
      - target: Taskbar.AugmentedEntryPointButton#AugmentedEntryPointButton > Taskbar.TaskListButtonPanel#ExperienceToggleButtonRootPanel
        styles:
          - Margin=4
          - Background:=$ElementBG
          - CornerRadius=12
      - target: Grid#SystemTrayFrameGrid
        styles:
          - Margin=0,7,20,7
          - RenderTransform:=<TranslateTransform X="-105" Y="-2"/>
          - Padding=0
          - Background:=$ElementBG
          - CornerRadius=12
      - target: SystemTray.ChevronIconView
        styles:
          - Padding=$TrayPadding
          - CornerRadius=10
      - target: SystemTray.NotifyIconView#NotifyItemIcon
        styles:
          - Padding=$TrayPadding
          - CornerRadius=10
      - target: SystemTray.OmniButton
        styles:
          - Padding=$TrayPadding
          - CornerRadius=10
      - target: SystemTray.CopilotIcon
        styles:
          - Padding=$TrayPadding
      - target: SystemTray.OmniButton#NotificationCenterButton > Grid > ContentPresenter > ItemsPresenter > StackPanel > ContentPresenter > systemtray:IconView#SystemTrayIcon > Grid
        styles:
          - Padding=$TrayPadding
      - target: SystemTray.IconView#SystemTrayIcon > Grid#ContainerGrid > ContentPresenter#ContentPresenter > Grid#ContentGrid > SystemTray.TextIconContent > Grid#ContainerGrid
        styles:
          - Padding=10
          - CornerRadius=10
      - target: SystemTray.StackListView#IconStack > ItemsPresenter > StackPanel > ContentPresenter > SystemTray.IconView#SystemTrayIcon
        styles:
          - Padding=0
      - target: SystemTray.Stack#ShowDesktopStack
        styles:
          - Visibility=Visible
      - target: Taskbar.Gripper#GripperControl
        styles:
          - Width=Auto
          - MinWidth=24
      - target: SystemTray.SystemTrayFrame
        styles:
          - HorizontalAlignment=1
          - RenderTransform:=<TranslateTransform X="399" />
      - target: Windows.UI.Xaml.Controls.Grid#AugmentedEntryPointContentGrid
        styles:
          - Margin=4,0,0,0
          - HorizontalAlignment=Left
      - target: TextBlock#TimeInnerTextBlock
        styles:
          - FontSize=13
          - FontFamily=vivo Sans EN VF
          - Margin=0
          - Padding=0
          - RenderTransform:=<TranslateTransform X="0" Y="0" />
      - target: TextBlock#DateInnerTextBlock
        styles:
          - Visibility=Collapsed
          - RenderTransform:=<TranslateTransform X="0" Y="-9" />
          - FontSize=11
          - FontFamily=vivo Sans EN VF
      - target: TextBlock#InnerTextBlock[Text=]
        styles:
          - Text=
      - target: Windows.UI.Xaml.Controls.Grid#ConfirmatorMainGrid
        styles:
          - CornerRadius=22
          - BorderThickness=$BorderThickness
          - BorderBrush:=$BorderBrush
          - Background:=$Background
      - target: TextBlock#SearchBoxTextBlock
        styles:
          - Text=Search This Precision
          - FontSize=10
          - FontFamily=vivo Sans EN VF
      - target: SystemTray.OmniButton#NotificationCenterButton > Grid > ContentPresenter > ItemsPresenter > StackPanel > ContentPresenter > SystemTray.IconView#SystemTrayIcon > Grid > Grid > SystemTray.TextIconContent
        styles:
          - Visibility=Collapsed
      - target: Windows.UI.Xaml.Controls.Button
        styles:
          - BorderThickness=$BorderThickness
      - target: Windows.UI.Xaml.Controls.Border#OverflowFlyoutBackgroundBorder
        styles:
          - BorderThickness=$BorderThickness
          - BorderBrush:=$BorderBrush
          - Background:=$Background
          - CornerRadius=$CornerRadius
      - target: WindowsInternal.ComposableShell.Experiences.Switcher.AltTab > Windows.UI.Xaml.Controls.Grid#ModalRootGrid > Border
        styles:
          - BorderThickness=$BorderThickness
          - BorderBrush:=$BorderBrush
          - Background:=Transparent
          - CornerRadius=20
      - target: WindowsInternal.ComposableShell.Experiences.Switcher.VirtualDesktopBarElement#VirtualDesktopBar
        styles:
          - //RenderTransform:=<TranslateTransform X="0" Y="60" />
          - CornerRadius=$CornerRadius
          - Background:=$Background
      - target: Windows.UI.Xaml.Controls.Border#BackgroundDimmingLayer
        styles:
          - Background:=$Background
      - target: Taskbar.TaskListButtonPanel#ExperienceToggleButtonRootPanel > Windows.UI.Xaml.Controls.Border#BackgroundElement
        styles:
          - CornerRadius=10
      - target: Taskbar.TaskListButton#TaskListButton
        styles:
          - CornerRadius=10
      - target: Windows.UI.Xaml.Controls.Border#SnapBarBorder
        styles:
          - Background:=$Background
          - BorderBrush:=$BorderBrush
          - CornerRadius=$CornerRadius
          - BorderThickness=$BorderThickness
          - RenderTransform:=<TranslateTransform X="0" Y="10" />
          - Margin=0,0,0,-10
      - target: Windows.UI.Xaml.Controls.Border#SnapPickerBorder
        styles:
          - Background:=$Background
          - BorderBrush:=$BorderBrush
          - CornerRadius=$CornerRadius
          - BorderThickness=$BorderThickness
      - target: Windows.UI.Xaml.Controls.Border#SearchPillBackgroundElement
        styles:
          - BorderBrush:=$ElementBorderBrush
          - CornerRadius=$ElementCornerRadius
          - BorderThickness=$ElementBorderThickness
          - Margin=0
      - target: Taskbar.TaskbarExtensionElement
        styles:
          - RenderTransform:=<TranslateTransform X="0" Y="0" />
      - target: Taskbar.TaskListButtonPanel#ExperienceToggleButtonRootPanel
        styles:
          - RenderTransform:=<TranslateTransform X="0" Y="0" />
      - target: Windows.UI.Xaml.Controls.ToolTip > Windows.UI.Xaml.Controls.ContentPresenter#LayoutRoot
        styles:
          - Background:=$Background
          - BorderBrush:=$BorderBrush
          - BorderThickness:=$BorderThickness
          - CornerRadius=12
      - target: SearchUx.SearchUI.SearchButtonControl
        styles:
          - MaxWidth=130
          - Margin=-1,0,-1,0
      - target: WindowsInternal.ComposableShell.Experiences.Switcher.VirtualDesktopBarElement > Windows.UI.Xaml.Controls.Grid#GridElement > Windows.UI.Xaml.Controls.Border#VirtualDesktopSwitcherBackground
        styles:
          - BorderBrush:=$BorderBrush
          - BorderThickness=$BorderThickness
          - CornerRadius=$CornerRadius
          - Background=Transparent
      - target: WindowsInternal.ComposableShell.Experiences.Switcher.SwitchItemListViewItem > Grid > Border
        styles:
          - Background:=Transparent
      - target: Border#VirtualDesktopBarBackground
        styles:
          - Background:=Transparent
          - BorderBrush:=$BorderBrush
          - BorderThickness=$BorderThickness
          - CornerRadius=$CornerRadius
    styleConstants:
      - Background=Transparent
      - BorderBrush2=Transparent
      - BorderThickness=0,0,0,0
      - CornerRadius=15
      - BorderBrush=Transparent
      - Background2=Transparent
      - TrayPadding=2
      - ElementBG=Transparent
      - ElementBorderThickness=0,0,0,0
      - ElementBorderBrush=Transparent
      - ElementCornerRadius=12
    resourceVariables:
      - variableKey: ''
        value: ''
    ```

    </details>

  - Advanced:

    <details>
    <summary>Click to expand</summary>

    ```json
    {
        "controlStyles[0].target": "Taskbar.TaskbarFrame#TaskbarFrame",
        "controlStyles[0].styles[1]": "HorizontalAlignment=Auto",
        "controlStyles[0].styles[2]": "Width=Auto",
        "controlStyles[0].styles[0]": "MaxWidth:=900",
        "controlStyles[0].styles[3]": "MinWidth:=500",
        "controlStyles[1].target": "Taskbar.TaskbarFrame#TaskbarFrame > Grid#RootGrid",
        "controlStyles[1].styles[0]": "Margin=30,0,30,5",
        "controlStyles[1].styles[1]": "BorderThickness=$BorderThickness",
        "controlStyles[1].styles[2]": "BorderBrush:=$BorderBrush",
        "controlStyles[1].styles[3]": "CornerRadius=$CornerRadius",
        "controlStyles[1].styles[4]": "Background:=Transparent",
        "controlStyles[2].target": "Rectangle#BackgroundFill",
        "controlStyles[2].styles[0]": "Visibility=Visible",
        "controlStyles[2].styles[1]": "Fill:=$Background",
        "controlStyles[3].target": "Rectangle#BackgroundStroke",
        "controlStyles[3].styles[0]": "Visibility=Collapsed",
        "controlStyles[4].target": "Taskbar.AugmentedEntryPointButton#AugmentedEntryPointButton > Taskbar.TaskListButtonPanel#ExperienceToggleButtonRootPanel",
        "controlStyles[4].styles[0]": "Margin=4",
        "controlStyles[4].styles[1]": "Background:=$ElementBG",
        "controlStyles[4].styles[2]": "CornerRadius=12",
        "controlStyles[5].target": "Grid#SystemTrayFrameGrid",
        "controlStyles[5].styles[0]": "Margin=0,7,20,7",
        "controlStyles[5].styles[1]": "RenderTransform:=<TranslateTransform X=\"-105\" Y=\"-2\"/>",
        "controlStyles[5].styles[2]": "Padding=0",
        "controlStyles[5].styles[3]": "Background:=$ElementBG",
        "controlStyles[5].styles[4]": "CornerRadius=12",
        "controlStyles[6].target": "SystemTray.ChevronIconView",
        "controlStyles[6].styles[0]": "Padding=$TrayPadding",
        "controlStyles[6].styles[1]": "CornerRadius=10",
        "controlStyles[7].target": "SystemTray.NotifyIconView#NotifyItemIcon",
        "controlStyles[7].styles[0]": "Padding=$TrayPadding",
        "controlStyles[7].styles[1]": "CornerRadius=10",
        "controlStyles[8].target": "SystemTray.OmniButton",
        "controlStyles[8].styles[0]": "Padding=$TrayPadding",
        "controlStyles[8].styles[1]": "CornerRadius=10",
        "controlStyles[9].target": "SystemTray.CopilotIcon",
        "controlStyles[9].styles[0]": "Padding=$TrayPadding",
        "controlStyles[10].target": "SystemTray.OmniButton#NotificationCenterButton > Grid > ContentPresenter > ItemsPresenter > StackPanel > ContentPresenter > systemtray:IconView#SystemTrayIcon > Grid",
        "controlStyles[10].styles[0]": "Padding=$TrayPadding",
        "controlStyles[11].target": "SystemTray.IconView#SystemTrayIcon > Grid#ContainerGrid > ContentPresenter#ContentPresenter > Grid#ContentGrid > SystemTray.TextIconContent > Grid#ContainerGrid",
        "controlStyles[11].styles[0]": "Padding=10",
        "controlStyles[11].styles[1]": "CornerRadius=10",
        "controlStyles[12].target": "SystemTray.StackListView#IconStack > ItemsPresenter > StackPanel > ContentPresenter > SystemTray.IconView#SystemTrayIcon",
        "controlStyles[12].styles[0]": "Padding=0",
        "controlStyles[13].target": "SystemTray.Stack#ShowDesktopStack",
        "controlStyles[13].styles[0]": "Visibility=Visible",
        "controlStyles[14].target": "Taskbar.Gripper#GripperControl",
        "controlStyles[14].styles[0]": "Width=Auto",
        "controlStyles[14].styles[1]": "MinWidth=24",
        "controlStyles[15].target": "SystemTray.SystemTrayFrame",
        "controlStyles[15].styles[0]": "HorizontalAlignment=1",
        "controlStyles[15].styles[1]": "RenderTransform:=<TranslateTransform X=\"399\" />",
        "controlStyles[16].target": "Windows.UI.Xaml.Controls.Grid#AugmentedEntryPointContentGrid",
        "controlStyles[16].styles[0]": "Margin=4,0,0,0",
        "controlStyles[16].styles[1]": "HorizontalAlignment=Left",
        "controlStyles[17].target": "TextBlock#TimeInnerTextBlock",
        "controlStyles[17].styles[0]": "FontSize=13",
        "controlStyles[17].styles[1]": "FontFamily=vivo Sans EN VF",
        "controlStyles[17].styles[2]": "Margin=0",
        "controlStyles[17].styles[3]": "Padding=0",
        "controlStyles[17].styles[4]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"0\" />",
        "controlStyles[18].target": "TextBlock#DateInnerTextBlock",
        "controlStyles[18].styles[0]": "Visibility=Collapsed",
        "controlStyles[18].styles[1]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"-9\" />",
        "controlStyles[18].styles[2]": "FontSize=11",
        "controlStyles[18].styles[3]": "FontFamily=vivo Sans EN VF",
        "controlStyles[19].target": "TextBlock#InnerTextBlock[Text=]",
        "controlStyles[19].styles[0]": "Text=",
        "controlStyles[20].target": "Windows.UI.Xaml.Controls.Grid#ConfirmatorMainGrid",
        "controlStyles[20].styles[0]": "CornerRadius=22",
        "controlStyles[20].styles[1]": "BorderThickness=$BorderThickness",
        "controlStyles[20].styles[2]": "BorderBrush:=$BorderBrush",
        "controlStyles[20].styles[3]": "Background:=$Background",
        "controlStyles[21].target": "TextBlock#SearchBoxTextBlock",
        "controlStyles[21].styles[0]": "Text=Search This Precision",
        "controlStyles[21].styles[1]": "FontSize=10",
        "controlStyles[21].styles[2]": "FontFamily=vivo Sans EN VF",
        "controlStyles[22].target": "SystemTray.OmniButton#NotificationCenterButton > Grid > ContentPresenter > ItemsPresenter > StackPanel > ContentPresenter > SystemTray.IconView#SystemTrayIcon > Grid > Grid > SystemTray.TextIconContent",
        "controlStyles[22].styles[0]": "Visibility=Collapsed",
        "controlStyles[23].target": "Windows.UI.Xaml.Controls.Button",
        "controlStyles[23].styles[0]": "BorderThickness=$BorderThickness",
        "controlStyles[24].target": "Windows.UI.Xaml.Controls.Border#OverflowFlyoutBackgroundBorder",
        "controlStyles[24].styles[0]": "BorderThickness=$BorderThickness",
        "controlStyles[24].styles[1]": "BorderBrush:=$BorderBrush",
        "controlStyles[24].styles[2]": "Background:=$Background",
        "controlStyles[24].styles[3]": "CornerRadius=$CornerRadius",
        "controlStyles[25].target": "WindowsInternal.ComposableShell.Experiences.Switcher.AltTab > Windows.UI.Xaml.Controls.Grid#ModalRootGrid > Border",
        "controlStyles[25].styles[0]": "BorderThickness=$BorderThickness",
        "controlStyles[25].styles[1]": "BorderBrush:=$BorderBrush",
        "controlStyles[25].styles[2]": "Background:=Transparent",
        "controlStyles[25].styles[3]": "CornerRadius=20",
        "controlStyles[26].target": "WindowsInternal.ComposableShell.Experiences.Switcher.VirtualDesktopBarElement#VirtualDesktopBar",
        "controlStyles[26].styles[0]": "//RenderTransform:=<TranslateTransform X=\"0\" Y=\"60\" />",
        "controlStyles[26].styles[1]": "CornerRadius=$CornerRadius",
        "controlStyles[26].styles[2]": "Background:=$Background",
        "controlStyles[27].target": "Windows.UI.Xaml.Controls.Border#BackgroundDimmingLayer",
        "controlStyles[27].styles[0]": "Background:=$Background",
        "controlStyles[28].target": "Taskbar.TaskListButtonPanel#ExperienceToggleButtonRootPanel > Windows.UI.Xaml.Controls.Border#BackgroundElement",
        "controlStyles[28].styles[0]": "CornerRadius=10",
        "controlStyles[29].target": "Taskbar.TaskListButton#TaskListButton",
        "controlStyles[29].styles[0]": "CornerRadius=10",
        "controlStyles[30].target": "Windows.UI.Xaml.Controls.Border#SnapBarBorder",
        "controlStyles[30].styles[0]": "Background:=$Background",
        "controlStyles[30].styles[1]": "BorderBrush:=$BorderBrush",
        "controlStyles[30].styles[2]": "CornerRadius=$CornerRadius",
        "controlStyles[30].styles[3]": "BorderThickness=$BorderThickness",
        "controlStyles[30].styles[4]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"10\" />",
        "controlStyles[30].styles[5]": "Margin=0,0,0,-10",
        "controlStyles[31].target": "Windows.UI.Xaml.Controls.Border#SnapPickerBorder",
        "controlStyles[31].styles[0]": "Background:=$Background",
        "controlStyles[31].styles[1]": "BorderBrush:=$BorderBrush",
        "controlStyles[31].styles[2]": "CornerRadius=$CornerRadius",
        "controlStyles[31].styles[3]": "BorderThickness=$BorderThickness",
        "controlStyles[32].target": "Windows.UI.Xaml.Controls.Border#SearchPillBackgroundElement",
        "controlStyles[32].styles[0]": "BorderBrush:=$ElementBorderBrush",
        "controlStyles[32].styles[1]": "CornerRadius=$ElementCornerRadius",
        "controlStyles[32].styles[2]": "BorderThickness=$ElementBorderThickness",
        "controlStyles[32].styles[3]": "Margin=0",
        "controlStyles[33].target": "Taskbar.TaskbarExtensionElement",
        "controlStyles[33].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"0\" />",
        "controlStyles[34].target": "Taskbar.TaskListButtonPanel#ExperienceToggleButtonRootPanel",
        "controlStyles[34].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"0\" />",
        "controlStyles[35].target": "Windows.UI.Xaml.Controls.ToolTip > Windows.UI.Xaml.Controls.ContentPresenter#LayoutRoot",
        "controlStyles[35].styles[0]": "Background:=$Background",
        "controlStyles[35].styles[1]": "BorderBrush:=$BorderBrush",
        "controlStyles[35].styles[2]": "BorderThickness:=$BorderThickness",
        "controlStyles[35].styles[3]": "CornerRadius=12",
        "controlStyles[36].target": "SearchUx.SearchUI.SearchButtonControl",
        "controlStyles[36].styles[0]": "MaxWidth=130",
        "controlStyles[36].styles[1]": "Margin=-1,0,-1,0",
        "controlStyles[37].target": "WindowsInternal.ComposableShell.Experiences.Switcher.VirtualDesktopBarElement > Windows.UI.Xaml.Controls.Grid#GridElement > Windows.UI.Xaml.Controls.Border#VirtualDesktopSwitcherBackground",
        "controlStyles[37].styles[0]": "BorderBrush:=$BorderBrush",
        "controlStyles[37].styles[1]": "BorderThickness=$BorderThickness",
        "controlStyles[37].styles[2]": "CornerRadius=$CornerRadius",
        "controlStyles[37].styles[3]": "Background=Transparent",
        "controlStyles[38].target": "WindowsInternal.ComposableShell.Experiences.Switcher.SwitchItemListViewItem > Grid > Border",
        "controlStyles[38].styles[0]": "Background:=Transparent",
        "controlStyles[39].styles[0]": "Background:=Transparent",
        "controlStyles[39].target": "Border#VirtualDesktopBarBackground",
        "controlStyles[39].styles[1]": "BorderBrush:=$BorderBrush",
        "controlStyles[39].styles[2]": "BorderThickness=$BorderThickness",
        "controlStyles[39].styles[3]": "CornerRadius=$CornerRadius",
        "styleConstants[0]": "Background=Transparent",
        "styleConstants[1]": "BorderBrush2=Transparent",
        "styleConstants[2]": "BorderThickness=0,0,0,0",
        "styleConstants[3]": "CornerRadius=15",
        "styleConstants[4]": "BorderBrush=Transparent",
        "styleConstants[5]": "Background2=Transparent",
        "styleConstants[6]": "TrayPadding=2",
        "styleConstants[7]": "ElementBG=Transparent",
        "styleConstants[8]": "ElementBorderThickness=0,0,0,0",
        "styleConstants[9]": "ElementBorderBrush=Transparent",
        "styleConstants[10]": "ElementCornerRadius=12"
    }
    ```

    </details>

5. Windows 11 File Explorer Styler

    Tùy chỉnh File Explorer với các chủ đề do người khác đóng góp hoặc tạo chủ đề của riêng bạn. Nói đúng là làm mờ thanh công cụ trong `Explorer`!

    __⚠️ Lưu ý__ Nếu dùng mod này thì mod `Translucent Windows` sẽ không còn trong suốt như đoạn code của tôi nữa mà sẽ chuyển thành đục mờ!

- Settings:

  <details>
  <summary>Click to expand</summary>

  ```yaml
  theme: Translucent Explorer11
  backgroundTranslucentEffect: ''
  backgroundTranslucentEffectRegion: ''
  controlStyles:
    - target: ''
      styles:
        - ''
  styleConstants:
    - ''
  themeResourceVariables:
    - ''
  explorerFrameContainerHeight: 0
  xamlDiagnosticsHandling: ''
  ```

  </details>

- Advanced:

  <details>
  <summary>Click to expand</summary>

  ```json
  {
      "backgroundTranslucentEffect": "none",
      "theme": "Translucent Explorer11",
      "controlStyles[0].target": "Grid#CommandBarControlRootGrid",
      "controlStyles[0].styles[0]": "Background=Transparent",
      "controlStyles[0].styles[1]": "BorderThickness=0",
      "controlStyles[1].target": "CommandBar#FileExplorerCommandBar",
      "controlStyles[1].styles[0]": "Background=Transparent",
      "controlStyles[2].target": "Grid#NavigationBarControlGrid",
      "controlStyles[2].styles[0]": "Background=Transparent",
      "controlStyles[3].target": "Grid#HomeViewRootGrid",
      "controlStyles[3].styles[0]": "Background=Transparent",
      "controlStyles[4].target": "FileExplorerExtensions.GalleryViewControl#GalleryViewControl > Grid",
      "controlStyles[4].styles[0]": "Background=Transparent",
      "controlStyles[5].target": "Microsoft.UI.Xaml.Controls.Grid#GalleryRootGrid",
      "controlStyles[5].styles[0]": "Background=Transparent",
      "controlStyles[6].target": "Grid#DetailsViewControlRootGrid",
      "controlStyles[6].styles[0]": "Background=Transparent",
      "explorerFrameContainerHeight": 0
  }
  ```

  </details>

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