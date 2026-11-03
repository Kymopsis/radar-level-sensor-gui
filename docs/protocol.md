# UART communication protocol

**Status: in preparation.** The full frame format will be published here.

What the boards support today (from the module datasheet):

- UART0, 115200 baud, 3.3 V logic: distance output and configuration commands.
- Distance output in metres, 1–5 reports per second; echo curve (512 FFT bins) on request; signal strength in dB.
- Configurable: range, blind zone, sensor offset, measurement interval (≥ 100 ms), report rate,
  address (1–247), false-echo learning (full, zone, remaining zone).

Until this page is complete, use the GUI to read and change settings.
