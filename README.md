# Hooklog
A C++ key logger program with multiple features.

This project was created for a 12th class CS project submission.

The program is a c++ based application which hooks to the keyboard to recieve all keystores and log them in a text file in a given directory.

Initial functions:

void sequencecall();
Calls other functions in a sequence

void relocation();
Relocates the program to specified directory by creating a batch with commands and executing it

int batcher(); // For the batch file containing relocation commands
Execute batch file using Createprocess()

void hide();
Hides the console window

void CreateFolder(const char * path);
Creates a folder in the specified directory

void addST();
Adds the program to startup registry 

void write(const char* c);
Writes the detected key to the log file

void send();
Function to upload the log file to ftp server

void KeepAlive();
Programs keeps running until hotkey / combination detected

void exit();

void recieveRB();
Downloads a (batch) file from remote ftp server to the specified directory (to be executed by the program)

void execute();
System command to open file

int executeprocess(); //For the downloaded remote file containing additional commands
Execute batch file using createprocess()

Note: This keylogger works by relocating itself to a custom directory named "JavaNET" when used for the first time IF not already in the specified directory
