# vidyo-ubuntu
Installing Vidyo on Ubuntu 16.04 LTS

1. Download Vidyo installer
```wget -O vidyo-desktop.deb https://goo.gl/2Ykmoq```

2. Run script
```./ vidyo-modify-deb.sh vidyo-desktop.deb```
3. Find and replace the line:

   ```Depends: libxss1,libaudio2,libasound2,libqt4-gui (>= 4.8.1), libqt4-network```

   with

   ```Depends: libxss1,libaudio2,libasound2,libqt4-designer,libqt4-opengl,libqt4-svg,libqtgui4,libqtwebkit4,libqt4-network```
4. Install the .modified.deb file
