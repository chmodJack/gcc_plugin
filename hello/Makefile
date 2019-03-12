INCLUDE=-I/usr/lib/gcc/x86_64-linux-gnu/6/plugin/include

all:main.c hello.so
	g++-6 $(INCLUDE) -shared -fPIC -o hello.so hello.c
	gcc-6 -fplugin=./hello.so main.c
