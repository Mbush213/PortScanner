# PortScanner
A Basic command-line port scanner written in python using built in socket and Re libraries 

How It Works
The script walks through three stages:

IP Validation — prompts the user for a target IP address and validates it against a regex pattern, looping until a properly formatted address is entered.
Port Range Selection — prompts for a port range in min-max format (e.g. 20-80), validates the input, and extracts the bounds.
Port Scanning — iterates over every port in the range, attempting a TCP connection to each one with a 0.5s timeout. Any port that accepts the connection is recorded as open and printed at the end.
