##
## This file is part of the libopencm3 project.
##
## Copyright (C) 2009 Uwe Hermann <uwe@hermann-uwe.de>
##
## This library is free software: you can redistribute it and/or modify
## it under the terms of the GNU Lesser General Public License as published by
## the Free Software Foundation, either version 3 of the License, or
## (at your option) any later version.
##
## This library is distributed in the hope that it will be useful,
## but WITHOUT ANY WARRANTY; without even the implied warranty of
## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
## GNU Lesser General Public License for more details.
##
## You should have received a copy of the GNU Lesser General Public License
## along with this library.  If not, see <http://www.gnu.org/licenses/>.
##

LIBNAME		= libopencm3_stm32f4

PREFIX	?= arm-none-eabi
# PREFIX		?= arm-elf
CC		= $(PREFIX)-gcc
AR		= $(PREFIX)-ar
CFLAGS		= -Os -g -Wall -Wextra -I../../../include -fno-common \
		  -mcpu=cortex-m3 -mthumb -Wstrict-prototypes \
		  -ffunction-sections -fdata-sections -MD -DSTM32F4
# ARFLAGS	= rcsv
ARFLAGS		= rcs
OBJS		= vector.o rcc.o gpio.o usart.o spi.o flash.o nvic.o \
		  i2c.o systick.o exti.o scb.o pwr.o timer.o \
		  usb.o usb_standard.o usb_control.o usb_fx07_common.o usb_f107.o \
		  usb_f207.o \

VPATH += ../../usb:../

include ../../Makefile.include
