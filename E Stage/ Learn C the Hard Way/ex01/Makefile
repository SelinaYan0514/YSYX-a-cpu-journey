CC = cc
CFLAGS = -Wall -Wextra -g
TARGET = build/main

$(TARGET): main.c
	mkdir -p build
	$(CC) $(CFLAGS) main.c -o $(TARGET)

run: $(TARGET)
	./$(TARGET)

output: $(TARGET)
	./$(TARGET) > output.txt

clean:
	rm -rf build output.txt

.PHONY: run output clean
