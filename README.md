# ESP32 workspace

1. clone an empty git repository named esp32-workspace
2. open vscode within the repository directory 
	```
	cd esp32-workspace/
	code .
	```
3. in vscode save current workspace within the git folder
   ```
   file --> save workspace as...
   ```
4. create projects folders from command line (not from vscode) within git folder
	```
   mkdir project1
   mkdir project2
   ```
5. open vscode and add `project1` and `project2` folders to workspace
   ```
   file --> add folder to workspace
   ```
6.  each project folder will contain its .vscode folder, a CMakeLists.txt file and README.md
	


## How build from command line
```bash
. $HOME/esp/esp-idf/export.sh
idf.py set-target esp32s3
idf.py build
idf.py -p /dev/cu.usbserial-14120 flash
idf.py -p /dev/cu.usbserial-14120 monitor # exit via ctrl + ]
idf.py -p /dev/cu.usbserial-14120 flash monitor # exit via ctrl + ]
```

Follow detailed instructions provided specifically for this example.

Select the instructions depending on Espressif chip installed on your development board:

- [ESP32 Getting Started Guide](https://docs.espressif.com/projects/esp-idf/en/stable/get-started/index.html)
- [ESP32-S2 Getting Started Guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s2/get-started/index.html)

