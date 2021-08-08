# KHFM Rando Tracker Backend

This repository contains the websocket server required for Co-Op/synchronisation in the [KH Rando Tracker frontend](https://github.com/zaxutic/kh-rando-tracker).

## Dependencies

- Python 3.6+
- `pip install -r requirements.txt`

## Running

```sh
python ws.py
```

While the server is running, it will display messages whenever rooms are created and closed (rooms are automatically closed once all clients disconnect from it). You can get information about all active rooms and how many clients are connected by sending a USR1 signal (e.g. `kill -s SIGUSR1 <PID>`)
