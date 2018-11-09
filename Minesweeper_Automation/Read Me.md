# Minesweeper Assistenace

This application helps to figure out the obvious move to help solve Minesweeper.

I tested the application against the Minesweeper in the below link:

http://minesweeperonline.com/


Before, execute the application you will need to install the below packages:

pip install pyobjc-core
pip install pyobjc-framework-Quartz
pip install image
pip install pyautogui
pip install pynput
easy_install pyscreenshot
pip install autopy
easy_install pyscreenshot

* If the application stuck and there is no obvious move, the application will hold on
and wait until a human/application to pick a random cell. 
* This application is designed to assist the 30x16 advanced minesweeper.
* The application starts by prompt the user to click on the top left then top right, to determine the game boundaries.
* Then, the application takes a snapshot of the game window defined in above step.
* The application divide the snapshot into grid of cells.
* For each cell, the application compare it to predefined cells to choose the best match to determine the type of the cell.
* After that, the application encodes the cell types into a matrix of numbers reflecting the cell types.
* Calculate the actions by defining the cells to be marked as mines.
* The application move the location of the mouse the these cells one by one.
* The simulate mouse right click, to mark the cell as mine.
* Finally, simulate click with both left and right mouse clicks to open the cell surrounding the marked cells.

** Repeate the above step until no action found, and prompt the users to fix the issue

** In future the application will be able to choose in random cells to open in case of no actions

https://github.com/ahmednassar/learn_python/tree/master/Minesweeper_Automation