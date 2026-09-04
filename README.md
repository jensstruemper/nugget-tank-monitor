# Nugget Tank Monitor

Capacitive fresh- and grey-water level monitoring for a Ford Nugget camper:
a Bluetooth LE controller board with two remote FDC1004 sensor heads, a
Zephyr firmware with over-the-air updates, and a Web Bluetooth page for
phone and laptop.

This public repository starts with the web page. Hardware and firmware
follow with the next board revision.

## Web page

`web/index.html` is a single, dependency-free page. It is served with
GitHub Pages at <https://jensstruemper.github.io/nugget-tank-monitor/>.

Web Bluetooth needs a secure context (HTTPS or localhost) and a browser
that supports it: Chrome or Edge on Android, Windows, macOS and Linux. On
iOS use the Bluefy app and open the page inside it.

For local development:

```sh
python3 -m http.server -d web 8000
```

then open <http://localhost:8000>.
