APPLICATION = mutex_order
include ../Makefile.tests_common

BOARD_INSUFFICIENT_MEMORY := stm32f0discovery weio nucleo-f030 nucleo32-f042 nucleo32-f031 \
                             nucleo-l053

include $(RIOTBASE)/Makefile.include

test:
# `testrunner` calls `make term` recursively, results in duplicated `TERMFLAGS`.
# So clears `TERMFLAGS` before run.
	TERMFLAGS= tests/01-run.py
