ARMGNU ?= arm-none-eabi

CC = $(ARMGNU)-gcc
LD = $(ARMGNU)-ld
AS = $(ARMGNU)-as
OBJCOPY = $(ARMGNU)-objcopy
OBJDUMP = $(ARMGNU)-objdump

LIBPI ?= ../../../../libpi

CPPFLAGS = -I$(LIBPI)/include
CFLAGS = -std=c99 -Wall -Og -g -ffreestanding $(CPPFLAGS) 
ASFLAGS =
LDFLAGS  = -nostdlib -T memmap -L$(LIBPI)/lib
LDLIBS = -lpi -lgcc

.SUFFIXES: 

NAME = main
SRCS = $(NAME).c

all : $(NAME).bin

%.o: %.s
	$(AS) $(ASFLAGS) $< -o $@ 

%.o: %.c
	$(CC) $(CFLAGS) -c $< 
	$(CC) -MM $(CFLAGS) -c $< > $*.d

%.elf: start.o cstart.o $(SRCS:.c=.o)
	$(LD) $(LDFLAGS) $^ $(LDLIBS) -o $@ 

%.bin: %.elf
	$(OBJCOPY) $< -O binary $@

%.list: %.o
	$(OBJDUMP) -d --no-show-raw-insn $< > $@

clean :
	rm -f *.bin
	rm -f *.elf
	rm -f *.o
	rm -f *.d
	rm -f *.list

install: $(NAME).bin
	rpi-install.py $(NAME).bin
	screen /dev/tty.SLAB_USBtoUART 115200

.PHONY : all clean

.PRECIOUS: %.elf %.o

# include dependency info 
#  "-" suppresses errors
-include $(SRCS:.c=.d)
