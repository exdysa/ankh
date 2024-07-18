# ankh
> 使用AppleScript快速操作，将MacOS通知中心等功能添加到正在运行的Scrcpy（https://github.com/Genymobile/scrcpy）。
> 
> AppleScript quick action for adding behavior like the MacOS notification center to a running [scrcpy](https://github.com/Genymobile/scrcpy
) window.
>
> (ANKH = ANC/Android無知中心/Android Nofitication Center)

https://github.com/user-attachments/assets/f1a8a9e2-f462-4654-87de-8fd2b119d901

## MacOS settings

> *将快捷操作分配给键盘命令，以便轻松启动。我在Multitouch（多指触控）中使用三点。
> *将分配到所有桌面（在“程序棒上下文菜单中的“选项”）。
> *可以轻松调整，适应任何应用程序作为边栏。
> *使用--window-borderless显示动画要更平滑，但仍然应该用边框做必须做的事情（显示和隐藏）。 MacOS安全功能干扰了屏幕边界外的窗口过渡效果。

> * Assign the quick action to a key command for effortless activation. I use a triple-tap in [multitouch](https://multitouch.app/)
> * Assign to all desktops (``'options'`` in dock context menu)
> * Could easily be adjusted to accomodate any app as a sidebar.
> * Appear animation is much smoother with --window-borderless, but it should still do what must be done (show and hide) with a border. MacOS security features interfere with window transition effects outside of screen bounds.

## Scrcpy启动设置示例 Example scrcpy Launch settings

> * 景觀 Landscape
> ```
> scrcpy -Sw --window-borderless -w --display-orientation=0 --window-y=24 --window-height=432 -m 1280 -K --always-on-top --window-borderless
> ```
> * 肖像 Portrait
> ```
>  scrcpy -Sw --window-borderless -w --window-y=24 --window-height=1256 -m 1152 -K --lock-video-orientation=0
>  ```
> * 圖示 Icon
> ```
> scrcpy --forward-all-clicks --window-x=-48 --window-y=24 --window-width=64 --window-height=48 --window-borderless --always-on-top -K
> ```
> * 全屏 Fullscreen
> ```
> scrcpy --forward-all-clicks --window-borderless -w --window-x=262
> ```



