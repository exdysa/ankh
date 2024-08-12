# ankh
> 蘋果煩俱接口快速動作，用於向運行中的scrcpy視窗添加類似MacOS通知中心的行為。
> （https://github.com/Genymobile/scrcpy）。
> 
> AppleScript quick action for adding behavior like the MacOS notification center to a running [scrcpy](https://github.com/Genymobile/scrcpy
) window.
>
> (ANKH = ANC/Android通知中心/Android Nofitication Center)

https://github.com/user-attachments/assets/f1a8a9e2-f462-4654-87de-8fd2b119d901

## MacOS settings

> 將快速動作指派給一個鍵盤命令，以便輕易啟用。我使用三次敲打在多點觸控中的方式。
> 將其指派給所有工作台（在儀表板上下文菜單中選擇“選項”）。
> 可以很容易地調整，以適應任何應用程序作為側欄。
> 出現動畫效果更加流畅時使用--window-borderless，但它仍然能夠完成所有必要的事情（顯示和隱藏），即使在具有框架的情況下。 MacOS安全性特性干擾了窗口過渡效果超出螢幕範圍之外的影響。

> * Assign the quick action to a key command for effortless activation. I use a triple-tap in [multitouch](https://multitouch.app/)
> * Assign to all desktops (``'options'`` in dock context menu)
> * Could easily be adjusted to accommodate any app as a sidebar.
> * Appear animation is much smoother with --window-borderless, but it should still do what must be done (show and hide) with a border. MacOS security features interfere with window transition effects outside of screen bounds.

## 例子：scrcpy啟動設定 Example scrcpy Launch settings

> * 景色 Landscape
> ```
> scrcpy -Sw --window-borderless -w --display-orientation=0 --window-y=24 --window-height=432 -m 1280 -K --always-on-top --window-borderless
> ```
> * 肖像 Portrait
> ```
>  scrcpy -Sw --window-borderless -w --window-y=24 --window-height=1256 -m 1152 -K --lock-video-orientation=0
>  ```
> *  圖標 Icon
> ```
> scrcpy --forward-all-clicks --window-x=-48 --window-y=24 --window-width=64 --window-height=48 --window-borderless --always-on-top -K
> ```
> * 全屏 Fullscreen
> ```
> scrcpy --forward-all-clicks --window-borderless -w --window-x=262
> ```



