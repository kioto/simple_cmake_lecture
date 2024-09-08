#
# 変数の定義
#

CXX		= g++
LDXX		= g++
CXXFLAGS	= -g -Wall
SRCS		= main.cpp
OBJS		= $(SRCS:.cpp=.o)
INCLUDES	= -I .
TARGET		= hello

#
# ルールの定義
#

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CXX) -o $(TARGET) $(OBJS)

.cpp.o:
	$(CXX) $(CXXFLAGS) -c $< $(INCLUDE) -o $@

main.o: main.cpp hello.h

clean:
	-rm -fr $(TARGET) $(OBJS) *~
