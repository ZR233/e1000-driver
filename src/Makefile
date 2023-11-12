# obj-m := e1000_for_linux.o

ARCH ?= x86_64

default:
	$(MAKE)  ARCH=$(ARCH) LLVM=1 -C $(KDIR) M=$$PWD

modules_install: default
	$(MAKE)  ARCH=$(ARCH) LLVM=1 -C $(KDIR) M=$$PWD modules_install