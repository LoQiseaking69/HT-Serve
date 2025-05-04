# HT-Serve

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)

HT-Serve is a secure HTTPS live reload server and dashboard prototyping tool. It is ideal for front-end and UI testing under realistic HTTPS conditions with dynamic refresh.

---

## Features

- Auto HTTPS with self-signed certs or custom cert path
- Live reload on file change
- CLI-driven orchestration (serve, check ports, reset demo)
- Template injection and dynamic dashboards
- Built-in test UI for development
- `/healthz` status endpoint
- Production logging and debug flags

---

## Installation

```bash
pip install .
```

---

## Usage

```bash
ht-serve serve --open-browser
ht-serve check
ht-serve reset-demo
```

---

## Environment Variables

| Variable         | Description                           |
|------------------|---------------------------------------|
| `DASH_CERT_PATH` | Path to HTTPS certificate             |
| `DASH_KEY_PATH`  | Path to HTTPS private key             |
| `DASH_PORT`      | Custom port to serve on (default 443) |
| `HT_DEBUG`       | Enable debug logging                  |
| `HT_FORCE_CERT`  | Force regenerate self-signed cert     |

---

## License

MIT © HermiTech Labs
