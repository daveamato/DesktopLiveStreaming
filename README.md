# #DesktopLiveStreaming
_loosely translated_

Knowing how to play live broadcast, **I wrote a small program** that will record the desktop and output audio and microphone of the machine, encoded as h264 and aac, and at the same time use the windows IOCP (I/O Completion Port) to create it easily A server that provides web services and live broadcast services, supports httpflv and hls live broadcast.

The following is the architecture diagram of the applet:
![](%23DesktopLiveStreaming/524900-20161119010854404-2135512941.jpg)

Run screenshot:
![](%23DesktopLiveStreaming/524900-20161119011500467-349608286.jpg)
 
**After starting, you can choose, fill in the port number and code rate, and then select the live broadcast method, and change the low screen to low api.**
 
![](%23DesktopLiveStreaming/524900-20170526151435107-515387608.png)
![](%23DesktopLiveStreaming/524900-20161119011508248-366933723.jpg)![](%23DesktopLiveStreaming/524900-20161119011516404-113547836.jpg)
 
![](%23DesktopLiveStreaming/524900-20161119011531779-1230335281.jpg)
 
Three libraries used by the program:
* **libx264** video encoding
* **libfaac** audio encoding
* **swscale** brga to yuv420
* 
_Note: xp system is not supported, please install dx11 first if the startup fails._