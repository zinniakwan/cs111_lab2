# cs111_lab2

## UID: 205777626

(IMPORTANT: Only replace the above numbers with your true UID, do not modify spacing and newlines, otherwise your tarfile might not be created correctly)

# A Kernel Seedling

Our kernel seedling counts the current number of processes running.

## Building

Use the following commands provided by the makefile:
make

## Running

Inject module into kernel:
sudo insmod proc_count.ko

To run:
cat /proc/count

What it does:
Once we inject the module into our /proc file, we count how many processes are running by incrementing a sum in the for_each_process command, and printing it out using the seq_printf command.

## Cleaning Up

You remove your kernel module with the terniman command:
sudo rmmod proc_count
make clean

## Testing

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on <https://www.kernel.org/>.
