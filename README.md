# ankh
> AppleScript quick action for adding behavior like the MacOS notification center to a running [scrcpy](https://github.com/Genymobile/scrcpy
) window.
>
> (ANKH = ANC/Android Nofitication Center)

## MacOS settings
> * Assign to all desktops (``'options'`` in dock context menu)

## Optional scrcpy Launch settings/

> * Landscape
> ```
> scrcpy -Sw --window-borderless -w --display-orientation=0 --window-y=24 --window-height=432 -m 1280 -K --always-on-top
> ```
> * Portrait
> ```
>  scrcpy -Sw --window-borderless -w --window-y=24 --window-height=1256 -m 1152 -K --lock-video-orientation=0
>  ```
> * Icon
> ```
> scrcpy --forward-all-clicks --window-x=-48 --window-y=24 --window-width=64 --window-height=48 --window-borderless --always-on-top -K
> ```
> * Fullscreen
> ```
> scrcpy --forward-all-clicks --window-borderless -w --window-x=262
> ```



