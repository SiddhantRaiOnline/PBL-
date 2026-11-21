# Northstar Airport Security Operations

A native Windows desktop application in C and C++. The GUI is drawn with Win32 and GDI; it does not open a browser or use a website.

## Build

Install MinGW GCC/G++ and ensure `gcc` / `g++` are on PATH. Open this folder in VS Code. Use **Ctrl+Shift+B** to build the C app, or **Terminal > Run Task** to select either C/C++ build or run task. The compiled EXEs are included.

## Menu sections

- **Overview:** checkpoint status and quick actions.
- **Passenger queue:** FIFO arrivals, add passengers, screen a batch.
- **Lane control:** view four lanes and auto-adjust capacity.
- **Incident desk:** simulate unattended-item, restricted-area, or crowd alerts; review and clear.
- **Baggage optimizer:** add sample bags and choose 15 kg check-in or 20 kg cargo limits.
- **Reports & metrics:** session totals and algorithm notes.
- **About:** algorithms, technology, and presenter details.

Baggage packing uses 0/1 knapsack, selecting whole bags to maximize carried weight without exceeding the selected limit. The desktop demo uses 3 kg, 5 kg, and 7 kg sample bag buttons. Alerts are simulated and do not process live CCTV or identify passengers.
