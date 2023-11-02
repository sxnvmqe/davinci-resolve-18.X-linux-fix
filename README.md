# davinci-resolve-18.X-linux-fix
Davinci Resolve (Studio) 18.X Linux error fixes.

### Tested on openSUSE Tumbleweed, Fedora 38 and Nobara 38.
Install depencies:

```
sudo zypper install libGLU1 libGLU1-32bit
```

Free:
```
cd ~/Downloads/
unzip ./DaVinci_Resolve_18.X_Linux.zip
chmod +x ./DaVinci_Resolve_18.X_Linux.run
sudo SKIP_PACKAGE_CHECK=1 ./DaVinci_Resolve_18.X_Linux.run -i
```

Studio:
```
cd ~/Downloads/
unzip ./DaVinci_Resolve_Studio_18.X_Linux.zip
chmod +x ./DaVinci_Resolve_Studio_18.X_Linux.run
sudo SKIP_PACKAGE_CHECK=1 ./DaVinci_Resolve_Studio_18.X_Linux.run -i
```

Fix errors:
```
cd /opt/resolve/libs
sudo mkdir _disabled/
sudo mv libgio-2.0.so* _disabled/
sudo mv libglib-2.0.so* _disabled/
sudo mv libgmodule-2.0.so* _disabled/
sudo mv libgobject-2.0.so* _disabled/
```

Fix errors: (After update)
```
cd /opt/resolve/libs
sudo rm -r _disabled/
sudo mkdir _disabled/
sudo mv libgio-2.0.so* _disabled/
sudo mv libglib-2.0.so* _disabled/
sudo mv libgmodule-2.0.so* _disabled/
sudo mv libgobject-2.0.so* _disabled/
```

## ENJOY VIDEO EDITING
