# Paperboat (`paperboat-paperboat`)

Showcase · autonomous sailing and upwind tacking · Python · port 8774

An interactive 3D sailing station for [Paperboat](https://github.com/paperboatlab/paperboat) that
proves custom HTML5 web stations, closed-loop upwind tacking control and aerodynamic sail trimming
in Python. The station serves an orthographic Three.js archipelago view over HTTP and streams
wind, boat state and waypoint telemetry to the Flow and Board over `paperboat/0`.

**Docs:** <https://paperboatlab.github.io/paperboat/tutorials.html>

## Run

```sh
paperboat run .
```

Or run the Python server directly with `paperboat` on `PYTHONPATH`:

```sh
python3 server.py --port 8774
```

Connect the Paperboat web app at `http://localhost:3047/?station=ws://localhost:8774`.

## Check

```sh
paperboat check .
paperboat pack .
```

## CI

[![package](https://github.com/paperboatlab/paperboat-paperboat/actions/workflows/package.yml/badge.svg?branch=dev)](https://github.com/paperboatlab/paperboat-paperboat/actions/workflows/package.yml?query=branch%3Adev) runs `paperboat check` and packages `paperboat-paperboat-<version>.pst`.
