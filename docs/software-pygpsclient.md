


### Enable User Port
In certain circumstances, users may need to manually configure the serial port for the application to function.

- **Pi 3/4/Zero 2W:**
	```shell
	sudo pygpsclient ---userport /dev/ttyS0
	```
- **Pi 5:**
	```shell
	sudo pygpsclient ---userport /dev/ttyAMA0
	```



### Desktop Application
The `pip` installation process does not automatically create a desktop application launcher, but this can be done manually:

https://github.com/semuconsulting/PyGPSClient/blob/master/APPLAUNCH.md


To create an application launcher for most Linux distributions, create a text file named `pygpsclient.desktop` with the following content (*adapted for your particular environment*) and copy this to the `/home/<user>/.local/share/applications` folder, e.g.




#### Adding to `PATH` Variable

If the Python 3 binaries folder is *not* in your PATH, you will need to add the fully-qualified path to the `pygpsclient` executable in the command above.

#### Find the directory of the relevant binaries
The location of the relevant binaries folder can usually be found by executing one of the following commands:

- If the package was installed in the virtual environment, activate it:
	```shell
	source <directory>/bin/activate
	```
- For a global installation, execute the following command:
	```shell
	python3 -c "import os,sysconfig;print(sysconfig.get_path('scripts'))"
	```
	The system should return the following directory for the relevant binaries, in a virtual environment:
	```shell
	/home/<user>/<directory>/bin
	```
- Deactivate, if inside a virtual environment:
	```shell
	deactivate
	```


!!! example
	For a virtual environment, to find the directory of the relevant binaries execute the following commands:

	```shell
	source env/bin/activate
	python3 -c "import os,sysconfig;print(sysconfig.get_path('scripts'))"
	deactivate
	```


<!-- Not a user installation!
Then, execute the following command for a user installation:
```shell
python3 -c "import os,sysconfig;print(sysconfig.get_path('scripts',f'{os.name}_user'))"
```

The system should return the following directory for the relevant binaries:
```shell
/home/<user>/.local/bin
```
-->



#### Add the directory to the `PATH` variable
To make the Python package accessible outside of the virtual environment, the directory of the relevant binaries need to be added to the `PATH` variable:


```shell
export PATH="$PATH:<directory to relevant binaries>"
```

!!! example
	```shell
	export PATH="$PATH:/home/pi/env/bin"
	```


```shell
source ~/.profile
```


<!-- Not a user installation!
!!! example
	```shell
	export PATH="$PATH:/home/<user>/.local/bin"
	```

	```shell
	export PATH="$PATH:~/.local/bin"
	```
-->


<!-- Application is not available system wide
```shell
source /etc/environment
```

```shell
source /etc/profile
```
-->


The application should now be available outside of the virtual environment:
```shell
pygpsclient
```


### Create Application Launcher
The `pip` installation process does not automatically create a desktop application launcher, but this can be done manually:

https://github.com/semuconsulting/PyGPSClient/blob/master/APPLAUNCH.md


To create an application launcher for most Linux distributions, create a text file named `pygpsclient.desktop` with the following content (*adapted for your particular environment*) and copy this to the `/home/<user>/.local/share/applications` folder, e.g.

```bash
[Desktop Entry]
Type=Application
Terminal=false
Name=PyGPSClient
Icon=/home/<user>/.local/lib/<python version>/site-packages/pygpsclient/resources/pygpsclient.ico
Exec=/home/<user>/.local/bin/pygpsclient
```

!!! example
	```bash
	[Desktop Entry]
	Type=Application
	Terminal=false
	Name=PyGPSClient
	Icon=/home/pi/.local/lib/python3.13/site-packages/pygpsclient/resources/pygpsclient.ico
	Exec=/home/pi/.local/bin/pygpsclient
	```


You will need to logout and login for the launcher to take effect.


desktop-file-validate <file_name>.desktop




### NTRIP Server



### NTRIP Caster

IP - address of Pi
Port - 2101
Mount - pygnssutils
user - anon
password - password

