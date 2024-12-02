# Chess Game GUI
A feature-rich Chess Game with a graphical user interface developed in Python using PySimpleGUI and Python-Chess modules. Players can challenge either another human player or an AI powered by Stockfish, a renowned chess engine. This project focuses on delivering an interactive and enjoyable chess experience while also providing tools for game analysis and saving[.

![image](https://github.com/user-attachments/assets/cbc879e5-ba0d-473d-affa-8fd3a0053219)

Command line to compile the source to exe using pyinstaller.

```
pyinstaller python_easy_chess_gui.py -F -w
```

Then add the folders for the exe to work.

## Features
* Play Against AI or Human Opponents: Challenge yourself against the Stockfish engine or enjoy casual games with another player.
* Game Saving and Loading: Save your games in industry-standard FEN or PGN formats and reload them anytime for analysis or resumption.
* AI-Powered Move Analysis: Get real-time advice and move evaluations to improve your gameplay.
* Interactive GUI: Simple and user-friendly graphical interface using PySimpleGUI for seamless gameplay.


Or you can just download the [executable file](https://github.com/fsmosca/Python-Easy-Chess-GUI/releases) along with other files such as book and images.

### B. Features
#### 1. Save games to repertoire pgn files
![](https://i.imgur.com/iXO2abq.png)

#### 2. Install uci engine of your choice
![](https://i.imgur.com/GErKZFy.png)

#### 2.1 It is recommended to configure the engine setting after installation
Configure engine via Engine->Manage->Edit, select engine and press modify.

![](https://i.imgur.com/PmDzCvz.png)

#### 3. Need book assistance? Right-click on BOOK 2 and press show
![](https://i.imgur.com/SdgNdr6.png)

#### 4. Need what engine adviser will think about the position? Right-click on Adviser and press start
![](https://i.imgur.com/Jziws5W.png)

### C. Installation
1. If you want to run from the source code
* Python Easy Chess GUI<br>
Download the files including the Images, Engines and Book directories. You can use your favorite uci chess engine like stockfish by copying it into the engines dir.
* Python 3<br>
https://www.python.org/downloads/
* Python-Chess<br>
https://github.com/niklasf/python-chess<br>
pip install python-chess
* PySimpleGUI<br>
https://github.com/PySimpleGUI/PySimpleGUI<br>
pip install pysimplegui
* Pyperclip<br>
https://github.com/asweigart/pyperclip<br>
pip install pyperclip
2. If you want to run from the exe
* Download the exe file from the release link

#### Note

If you are on linux be sure to give permission to uci engine with:  
`chmod +x uci_engine_fn`.

### D. How to
#### To start the gui
* Execute python_easy_chess_gui.py<br>
Typical command line:<br>
`python python_easy_chess_gui.py`
* Execute the exe when using exe file

#### To play as white
* Mode->Play
* Move the piece you want to move
* Press the square you want the piece to move to

#### To play as black
* If current mode is Neutral, Board->Flip, flip such that black pieces are at the bottom
* If current mode is Play, Mode->Neutral, then Board->Flip
* Mode->Play
* Engine->Go

#### To paste a FEN
* You should be in Play mode. If not, then Mode->Play
* FEN->Paste
* If you play as white, you can make your move
* If you play as black, Engine->Go

#### To flip board
* If current mode is Neutral, Board->Flip
* If current mode is Play, Mode->Neutral, then Board->Flip

#### To set opponent engine book options
* Book->Set Book, only available in Neutral mode. This book is used by your opponent engine. This book is named pecg_book.bin and is located in Book folder. You can build a polyglot book name it pecg_book.bin and replace the default.

#### To Hide/Unhide engine search info
* Right-click on Opponent Search Info label an press Show. This would only work on Play mode.

#### To Hide/Unhide Book info
* Right-click on BOOK 1 or BOOK 2 labels and press Show. This would only work on Play mode.

#### To request Adviser search info
* Right-click on Adviser and press start. This would only work on Play mode.

#### To select opponent engine
* Engine->Set Engine Opponent, available only in Neutral mode.

#### To set time control of engine
* Time->Engine

#### To set time control of user
* Time->User

#### To install engine
* Engine->Manage->Install  
This is only accessible in Neutral mode. After the uci engine is installed, you have to Edit it to modify its options, etc. Only uci engines are supported so far.
* Engine->Manage->Edit

#### To Edit engine
* Engine->Manage->Edit

#### To delete engine from config file
* Engine->Manage->Delete

### E. Credits
* PySimpleGUI<br>
https://github.com/PySimpleGUI/PySimpleGUI
* Python-Chess<br>
https://github.com/niklasf/python-chess
* Pyperclip<br>
https://github.com/asweigart/pyperclip
* The Week in Chess<br>
https://theweekinchess.com/
* PyInstaller<br>
https://github.com/pyinstaller/pyinstaller
* pgn-extract<br>
https://www.cs.kent.ac.uk/people/staff/djb/pgn-extract/
