# zinit -- Use `zram` for your rootfs

## Usage

1. Install `zinit` to `/sbin` or some other place where your
   kernel can find it.
1. Make sure you can `modprobe zram` before executing `init`.
1. Modify the constants in the configuration block.
1. Tell your bootloader to add the option `init=/sbin/zinit` to
   your kernel's boot command line

## Rationale

You boot your computer rarely, you execute programs often. Don't
do this if you have insufficient main memory.
