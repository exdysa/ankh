# ankh
> 蘋果煩俱接口快速動作，用於向運行中的scrcpy視窗添加類似MacOS通知中心的行為。
> （https://github.com/Genymobile/scrcpy ）
> 
> AppleScript quick action for adding behavior like the MacOS notification center to a running [scrcpy](https://github.com/Genymobile/scrcpy
) window.
>
> (ANKH = ANC/Android通知中心/Android Nofitication Center)

https://github.com/user-attachments/assets/f1a8a9e2-f462-4654-87de-8fd2b119d901

## MacOS setup

> * 在终端运行以下命令来添加环境和别名到zsh。
```
echo -e "\n# ankh + scrcpy\nexport PATH='$PATH:/usr/local/Cellar/scrcpy/2.6.1/bin/scrcpy:/usr/local/Caskroom/android-platform-tools/35.0.1/platform-tools/'\nankh(){\n scrcpy -Sw -w --window-y=24 --max-fps=30 -b 4M  -m 1152 -K --always-on-top  --window-borderless --window-height=\"\$1\" \n}\n" >> ~/.zprofile
```
> 确保路径和启动设置与您对scrcpy期望的质量设置相匹配。更多设置请参阅scrcpy设置。(https://github.com/Genymobile/scrcpy#user-documentation)
> 请确保路径和启动设置与您所欲的scrcpy质量设置相匹配。查看scrcpy设置以获取更多设置。

> 將快速動作指派給一個鍵盤命令，以便輕易啟用。我使用三次敲打在多點觸控中的方式。
> 將其指派給所有工作台（在儀表板上下文菜單中選擇“選項”）。
> 可以很容易地調整，以適應任何應用程序作為側欄。
> --window-borderless 窗口边框为空时，动画效果更加流畅，但它仍然应该在必要时执行（显示和隐藏）带有边框。MacOS安全功能会干扰窗口过渡效果超出屏幕范围内的情况。

> * Run the following command in `Terminal` to add the environment and alias to `zsh`.
```
echo -e "\n# ankh + scrcpy\nexport PATH='$PATH:/usr/local/Cellar/scrcpy/2.6.1/bin/scrcpy:/usr/local/Caskroom/android-platform-tools/35.0.1/platform-tools/'\nankh(){\n scrcpy -Sw -w --window-y=24 --max-fps=30 -b 4M  -m 1152 -K --always-on-top  --window-borderless --window-height=\"\$1\" \n}\n" >> ~/.zprofile
```
> Be sure the path and launch settings match your desired quality settings for `scrcpy`. See the [scrcpy settings](https://github.com/Genymobile/scrcpy#user-documentation) for more settings.

> * Assign the quick action to a key command for effortless activation. I use a triple-tap in [multitouch](https://multitouch.app/)
> * Assign to all desktops (``'options'`` in dock context menu)
> * Could easily be adjusted to accommodate any app as a sidebar.
> * Appear animation is much smoother with --window-borderless, but it should still do what must be done (show and hide) with a border. MacOS security features interfere with window transition effects outside of screen bounds.

> Thank you for using it. 有我的贡献能給你帶來幸福是榮幸.

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



