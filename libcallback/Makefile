# libcallback.so

CC = /atomtools/build/mips-gcc472-glibc216-64bit/bin/mips-linux-uclibc-gnu-gcc
CFLAGS = -fPIC -std=gnu99 -shared -ldl -ltinyalsa -lm
CC_SRCS = video_callback.c audio_callback.c jpeg.c setlinebuf.c mmc_format.c curl.c freopen.c opendir.c remove.c motor.c command.c gmtime_r.c wait_motion.c irled.c audio_play.c mp4write.c usb_power.c timelapse.c
TARGET = libcallback.so

all: ${TARGET}

${TARGET}: ${CC_SRCS}
	${CC} ${CFLAGS} -o ${TARGET} ${CC_SRCS}
