# Porn Fetch

#### We all know that feeling when we try to download something from Pornhub and then we go to our Search Engine and what we find is shady websites, with too much ads and payment concepts in it. I decided to fuck this shit and now I created it by myself.

# API

### I am using the [PHUB](https://github.com/Egsagon/PHUB) API from Egsagon. This Project would not be possible without this AWESOME API

## Is this legal? 

I don't know about the law in your country. I can only say in Germany it's allowed to download 7 copyright licensed materials.
Also, you need to be at least 18+ years old to watch (and have) Porn videos. I am not liable for anything! You know what you do

# GUI

The Graphical User Interface was created with PySide6 (Qt for Python)
# Releases

Some releases are too big for GitHub. In that case, you can find it on [Google Drive](https://drive.google.com/drive/folders/1sGvhAO_qQB87AOfyVDWPJZluVettBwaj?usp=sharing)

# Other Infos

- ### If Progressbar gets stuck, this is normal. Just wait.
- ### Output path must contain a slash at the end

# Building from Source

- Download a Version of Python 3.X along with pip (I did all this with Python 3.11.4)
- Clone the project with git or using the zipfile
- Install needed pip packages: pip (or pip3) install pyside6 phub wget colorama pyinstaller
- git clone https://github.com/EchterAlsFake/Porn_Fetch
- cd Porn_Fetch
- pyinstaller -F widget.py
- In you dist directory, there is the executable file

# What about Android?

It is possible to compile a PySide6 application like mine to Android. There is one official guide from the Qt company about it.
The problem is, that my Arch is just broken and not working well. Many packages are missing for the compilation and I can not use
my Python3.11 for it and switching to Python3.10 is (in this case) more than just $ sudo make altinstall ;) 
If you want to give it a try, here is the guide: https://www.qt.io/blog/taking-qt-for-python-to-android<br>
I am experimenting with it, and I let you know about the progress.

# Changelog

## 1.0 

- Initial Release 

## 1.1

- Code refactoring
- Added Support for downloading a whole channel / user
- Fixed an Issue with the progress bar
- Fixed typo issues
- Fixed the output path issue
- Changed License to LGPLv3  (The reason for this is, that I am stupid and I used the wrong license. Creative Commons is not valid to be used for developing with Qt. I didn't know that, I am sorry...)

## 1.2

- Added additional stuff to the metadata function (Likes, Image URL, Tags)
- Added border colours for input fields

## 1.3

- Added Threading Modes

Single: Downloads will be executed within the main thread, and the GUI
won't respond to your actions if the download isn't finished.

Multiple: Download(s) will be executed with separate Threads (QThreads). This is mostly intended for single downloads. You can use that function also for multiple downloads, but that will ruin the progress bar, because it will jump between the different videos. 

Your decision ;)

# Contributing

You can contribute literally everything. Typo Errors, code optimization, features... Just make a Pull Request :) <br>

# Credits

- Thanks to Egsagon for creating the PHUB API <br>
- Thanks to Qt for making PySide6 :) <br>
- Thanks to Pyinstaller for compiling stuff <br>

# License

Porn Fetch 2023 by Johannes Habel LGPLv3 License

-- Attention -- You need to Credit Egsagon for his API and me Johannes Habel for the project

This is just an act of kindness. Thanks :) 
