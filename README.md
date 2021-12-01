Getting started with ESP 32 in Arduino IDE

1. go to
	https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/
	
2. Installing PIP 3
	sudo add-apt-repository universe
	sudo apt install python3-pip
	
3. Solving problem of importing serial
	sudo apt install python-is-python3
	
4. Solving the problem associated with permission denial (arduino [Errno 13] Permission denied: '/dev/ttyUSB0')
	Run the code 
	sudo chmod a+rw /dev/ttyUSB0
	
Replacing the custom U8G2 driver configuration for arduino with that for ESP32
	U8G2_ST7920_128X64_F_SW_SPI u8g2(U8G2_R0, /* clock=*/ 18, /* data=*/ 23, /* CS=*/ 5, /* 		reset=*/ 22); // ESP32 

