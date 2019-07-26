+++
Date = "2017-01-30"
TagLine = "Windows 10 app"
Title = "Screen Recordr"
SubTitle = "Screen capture app"
Thumbnail = "assets/img/app/screen-recordr/thumb.png"
Images = [
  "assets/img/app/screen-recordr/desktop01.png",
  "assets/img/app/screen-recordr/desktop02.png",
]
WinStoreAppId = ""
WebLink = ""
+++

# No-nonsense screen video capture for Windows 10

I never really liked OBS and the myriad other dodgy desktop recording apps for Windows even less, so now that UWP has a screen capture API I decided to make my own. I also like Fluent Design so enjoy the Acrylic. If the app looks like a copy of Voice Recorder it's very much on purpose :)

# Screen Recordr records a desktop or a single application window to MP4 and that's it

But is's fast and stays out of the way as you do. No ads. No telemetry. No bullshit.

Encoding is handled by MediaFoundation, Windows's native API: if your GPU has a dedicated video encode block and a proper driver, it should just work. This should apply to Windows on ARM devices as well and Screen Recordr is compiled for x86/x64/ARM/ARM64, so you get native speed no matter what device you are on.

CPU usage is in the ~1% range when encoding 4Kp60. If you have issues try upgrading your video drivers first.