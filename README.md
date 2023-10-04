# PLANET-AI
Integration of recognition engine of PLANET-AI into Kofax Transformation

## Installation and Configuration
* download and unzip **IDA_Server_5.1.1_windows.zip**.
* at Admin Command prompt run **installAsWindowsService.bat** from it's folder.
* Add your customer id at the command prompt when requested.
### Python
* Install Visual Studio Code.
* Load the folder **grpc_process_image_v2** into VSCode.
* VSCode will prompt you to install Python Plugin.
* Open file **process_image_request.py** in VSCode.
* Press F5 to debug. VSCode will ask for your Python interpreter and take you to Microsoft Store to download Python 3.11.
## Test Document
* Press F5 to debug.
* if you get error **Import "grpc" could not be resolved.
  * Open Terminal from View/Terminal (CTRL-').
  * Type **pip install grpcio** to install Google's [Remote Procedure Call](https://en.wikipedia.org/wiki/GRPC) framework. You should see *Successfully installed grpcio-1.59.0*.
  * Type **pip install grpcio-tools** to install Google's [Remote Procedure Call](https://en.wikipedia.org/wiki/GRPC) framework. You should see *Successfully installed grpcio-1.59.0*.

  ## Reverse Engineering REST Service
* the following curl command successfully logs into the IDA Cockpit. It ignores the certificate.
```cmd
curl -k  --header "Content-Type: plain/text"  --data-raw "username=admin&password=password"  https://localhost:8004/
```  
