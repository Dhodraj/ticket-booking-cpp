# ticket-booking-cpp

A command-line bus ticket booking system in C++. An admin, such as a conductor, signs in and books, cancels and views tickets across five routes.

Built in 2021, as a mini project.

## What it does

- Sign up and log in. A password must be eight characters or more.
- View the bus list: Salem to Erode, Ooty, Kodaikkanal, Coimbatore and Chennai.
- Book tickets, and confirm after a payment step.
- Cancel booked tickets.
- View seat status for a route.

It keeps everything in memory for one run, so bookings do not persist after you exit.

## Build and run

```bash
g++ bus.cpp -o bus
./bus
```

The code uses `conio.h` and `getch()`, so it builds as is with Windows compilers such as MinGW. On Linux or macOS, replace those before building.

To make the login page the entry point, change the first call in `main()` to `first()`.
