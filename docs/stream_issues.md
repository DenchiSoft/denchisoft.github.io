# Why does my stream to PC/Mac lag?

[\[Back to main page\]](https://denchisoft.github.io/)

Under normal circumstances, there should be no delay, lag or hickups/spikes. The streaming should be smooth and should have at most around 10 milliseconds of delay.

However, depending on your local network setup, there might be some issues.

## Network Troubleshooting (general)
- Are you on WiFi? Your WiFi reception may cause lag or even very long (multiple seconds) delays in packets being sent over your network. Make sure you use 5GHz WiFi and not 2.4 as depending on your environment, 2.4 Ghz WiFi can have wildly unstable latency. With WiFi, the latency still shouldn't be higher than 10 milliseconds.
- If possible, use wired LAN connection instead of WiFi. This will give you a lag-free, 1-ms latency connection. You can use wired LAN on your smartphone using an adapter such as [this one for Android (USB-C)](https://www.amazon.com/dp/B0823CB5MT/ref=cm_sw_r_tw_dp_U_x_tE-VEbHCNDE1B) or [this one for iPhone](https://www.amazon.com/dp/B07TNDBB2X/ref=cm_sw_r_tw_dp_U_x_4C-VEb5BWZ0KC).
- Try restarting your router. That sometimes helps.

## Network Troubleshooting (macOS and iPhone)
- Turn off location services, they will cause lag spikes periodically when your Mac scans your environment for WiFi networks. To turn that off, follow [this guide](https://osxdaily.com/2018/08/20/disable-location-services-mac/).
- If you're using WiFi, remove all unused WiFi-Networks from your list of known networks on both iPhone and Mac to stop them from scanning for them constantly. You can follow [this guide](https://9to5mac.com/2018/07/20/mac-how-to-forget-wireless-networks/).
- When using iPhone and MacBook on WiFi: __Very important to turn off AirDrop on the
Macbook__, because it __WILL__ cause massive lag spikes when the iPhone is close to the Mac. Open a console and type:
  - __sudo ifconfig awdl0 down__
- Later, when you're done streaming, you can turn it back on by rebooting your Mac or typing this in a console:
  - __sudo ifconfig awdl0 up__
- Turning off Bluetooth on your Mac and iPhone can also help. You can follow [this guide](https://support.apple.com/guide/mac-help/turn-bluetooth-on-or-off-blth1008/mac) to turn of Bluetooth on your Mac.

