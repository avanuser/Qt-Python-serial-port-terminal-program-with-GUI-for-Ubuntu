# qt-gsm-terminal_ubuntu
Qt Python serial port GSM terminal with GUI for Ubuntu

This is a terminal program with GUI communicating through serial port.
It can be used to facilitate testing of any cellular (2G/3G/LTE/etc) or any other modems controlled by AT-like commands.

This program is modified for use with Ubuntu OS (sucsessfully tested with Ubuntu 20).

To get information about serial ports use "Ports info" button.
To get list of free serial ports use "Get free ports" button.
To open serial port enter number of the port (digits only) in "Port number" field and press "Open" button.
In case of empty "Port number" field the program will open first free port with the lowest number.

If you need to migrate from PySide6 to PySide2 just rename "PySide6" to "PySide2" in imports and change the following lines at the end of main.py:

\# sys.exit(app.exec())  # PySide6

sys.exit(app.exec_())   # PySide2


![Qt Python serial port GSM terminal](https://github.com/avanuser/qt-gsm-terminal_ubuntu/blob/main/qt_gsm_terminal_ubuntu.png)
