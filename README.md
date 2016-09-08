# bpi-health-dashboard

This repository contsins a modified Python sensor script for [pi-health-dashboard](https://github.com/initialstate/pi-health-dashboard) to work with a Banana Pi.

Since all the sensor values except from temperature are provided by `psutil`, most of the script is compatible with a Banana Pi out-of-the-box. The only issue is the temperature, which is retrieved using `vcgencmd` on a Raspberry Pi, but this is not available on the Banana Pi. However, this can be easily replaced with `lm-sensors`.

## Instructions

If you don't have it already, install `lm-sensors`:
```
$ sudo apt-get install lm-sensors
```

Then, simply follow the original tutorial (available below).

---

![Pi System Health Dashboard](https://github.com/InitialState/pi-health-dashboard/wiki/img/dashboard_final.gif)

This is a hub for the System Health Dashboard for your ~~Raspberry~~ Banana Pi project.

Here you will find code materials for the tutorial as well as the tutorial itself in the [wiki](https://github.com/InitialState/pi-health-dashboard/wiki).

~~Raspberry~~ Banana Pis are being used to drive a ridiculous number of projects ranging from fun hobby projects to mission critical functions. Despite being small, user-friendly, and inexpensive, your Pi contains an impressive number of complex subsystems that must work to keep your project running. This makes being able to monitor the health of your Pi important in many applications from ongoing maintenance of a long-term project to profiling the performance of a new prototype ... [read more](https://github.com/InitialState/pi-health-dashboard/wiki)

