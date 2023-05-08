# cs111_lab2

## UID: 205777626

# You Spin Me Round Robin

Our C project simulates the "round robin" implementation of CPU scheduler. The program outputs the overall average waiting time and repsonse time of a series of processes, which the user inputs for a certain time quantum.

Round Robin is a scheduling algorithm that places incoming processes into a queue, and exectues them in FIFO for the allotted quantum time.

## Building

Use the following commands provided by the makefile:
make

## Running

We must include a txt file path that specifies the proccess ids, arrival times, and burst times as our first argument.
We must also specify the quantum length as our second argument.

For example, if we are trying to access processes in processes.txt with a quantum time of 3, we run:

./rr processes.txt 3

## Cleaning Up

run the following command: make clean
