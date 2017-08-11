This is the configuration file for the wl1837 module.

It was created using the `configure-device.sh` script from TI (it can be found
on the BeagleBone Wireless Green image at `/usr/share/ti/wlconf`).

This configuration enables 5 GHz support on the radio.

`wl18xx-conf.bin` should be placed into `/lib/firmware/ti-connectivity`.

Also note: if the `wlan0` interface says "Cannot assign requested address" or
something similar, this is due to an invalid MAC being set. Remove
`/lib/firmware/ti-connectivity/wl1271-nvs.bin`.