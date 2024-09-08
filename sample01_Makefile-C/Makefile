#
# 変数の定義
#

CC		= gcc
LD		= gcc
CFLAGS		= -g -Wall
SRCS		= main.c
OBJS		= $(SRCS:.c=.o)
INCLUDES	= -I .
TARGET		= hello

#
# ルールの定義
#

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CC) -o $(TARGET) $(OBJS)

.c.o:
	$(CC) $(CFLAGS) -c $< $(INCLUDE) -o $@

main.o: main.c hello.h

clean:
	-rm -fr $(TARGET) $(OBJS) *~
