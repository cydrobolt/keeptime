## keeptime :recycle: :clock1:
Keep tabs on the time by hearing the time spoken.
keeptime is a lightweight tool to help reduce procrastination.

```
usage: keeptime [-h] [-d] [-l LANG] [-q]

optional arguments:
  -h, --help            show this help message and exit
  -d, --daemon          run keeptime as a daemon
  -l LANG, --lang LANG  two-letter language code for localization
  -q, --quarter         say time every quarter hour
```


Example: `./keeptime -d -l en`

By default, keeptime announces the time every 30 minutes. However, you can increase the frequency using `-q` to announce the time every quarter hour.

### Running keeptime
 - Clone the repository
 - Install dependencies (`pip install -r requirements.txt`)
 - Ensure `ffmpeg` or `libav` is installed
 - Run `./keeptime <lang_code>` (e.g `./keeptime en`)
 - Add an auto start entry (e.g in GNOME) to start keeptime on boot

### Running keeptime on startup
 - Copy the repository to `~/.local/share/keeptime`
 - Add `keeptime.desktop` to `~/.local/share/applications/`
 - Add `keeptime.desktop` to your auto start applications (e.g in GNOME Tweak Tool)
