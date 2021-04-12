# Time's Up

<p align="left">
 <a href="https://snapcraft.io/teatime"><img src="https://img.shields.io/badge/based%20on-Teatime-ff69b4"></a>
 <img alt="GitHub" src="https://img.shields.io/github/license/roxennnn/TimesUp">
</p>

**Time's Up** is an application developed to help computer users take care of their eyes. After a long time staring at their screens, computer users &ndash; who can be developers, analysts, youtubers, whoever &ndash; need to take a break and look somewhere else. Time's Up has been devised to remind and "force" users to take a break after a certain period of time. 

Time's Up consists of a timer which, when it expires, displays a desktop notification to the user reminding her to take a break. After a pre-defined period of time (by default, it corresponds to 5 minutes) if the user have not locked the screen yet, the application will automatically lock the computer screen. 

This application is based on [Teatime](https://snapcraft.io/teatime) by [Pavel Rojtberg](https://github.com/paroj). Teatime is "*a simple egg-timer type application to time your teas. Rings an alarm and displays a desktop notification, when the tea is ready*".


## Usage

Time's Up has been tested working only on Linux. In particular, it has been tested working on Ubuntu 18.04 (GNOME) and on Linux Mint 20 (Cinnamon).

Time's Up is written in Python3.

### Install dependencies
```bash
pip3 install requirements.txt
```

### Run application
```bash
python3 timesup.py
```

### App usage
When the app starts, a 1 hour timer (default) is started.

To add a new timer, click on "*Create a New Timer*", then type name and duration for the new timer. To modify an existing timer, follow the previous procedure. To delete a timer, instead, select a timer and press "Del". Timers are stored in `config/store.json`.

## Possible configurations
The following configuration parameters can be changed from the `config/constants.json` file.

* `remind_delta_seconds`: pre-defined period of time in seconds from when the timer expires and when the screen is "forced" to be locked; default is `300`.
* `sound_alert_file`: sound played when timer expires; default is `/usr/share/sounds/freedesktop/stereo/service-login.oga`.
* `sound_lock_file`: sound played when screen is locked; default is `/usr/share/sounds/freedesktop/stereo/service-logout.oga`.


## Future Improvement Ideas

In the following some ideas to improve Time's Up are listed.
* Make it work for other OSes, starting from Windows
* Improve user interface, maybe using a different technique
* Add theming and other customisation settings, like:
  * Set default starting timer
  * Activate or deactivate default timer on start

## License
[MIT](https://github.com/roxennnn/TimesUp/blob/master/LICENSE)

## Acknowledgements

Thanks to my mum for her precious support.
