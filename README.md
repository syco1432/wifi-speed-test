# WiFi Speed Test

A lightweight Python tool that measures your internet connection: **ping**, **download speed**, and **upload speed**. It uses only Python's standard library, so there is nothing extra to install.

## Features

- Ping test with average, minimum, and jitter
- Download speed in Mbps
- Upload speed in Mbps
- No external dependencies
- Works on Windows, macOS, and Linux

## Requirements

- Python 3.6 or newer
- An active internet connection

## Usage

1. Clone the repository or download `speedtest.py`:

   ```bash
   git clone https://github.com/syco1432/wifi-speed-test.git
   cd wifi-speed-test
   ```

2. Run the script:

   ```bash
   python speedtest.py
   ```

## Example Output

```
========================================
        WiFi Speed Test
========================================
Testing ping...      32.4 ms (min 28.1 ms, jitter 3.2 ms)
Testing download...  45.60 Mbps
Testing upload...    12.35 Mbps
----------------------------------------
Ping     : 32.4 ms
Download : 45.60 Mbps
Upload   : 12.35 Mbps
========================================
```

*(Your numbers will differ depending on your connection.)*

## How It Works

The script connects to Cloudflare's public speed test servers:

- **Ping:** times several tiny requests and reports the average, minimum, and jitter.
- **Download:** downloads a 25 MB file and calculates the speed from the time taken.
- **Upload:** uploads 10 MB of random data and calculates the speed from the time taken.

## Notes

- Results can vary between runs. Run it a few times for a better idea of your real speed.
- For accurate results, close other apps and downloads that use the internet.
- Connect closer to your router or use a cable to compare WiFi vs. wired speed.

## License

Free to use and modify.
