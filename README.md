# Set_password_at_Terminal
Want to secure the terminal (Mac, Linux, windows not tested yet), give it a try at your own risk. 

Req. Libraries: Anaconda, opencv, termcolor

Caution: It uses the computer camera and takes a snap after three consecutive faliure while providing an user name and password. The snaps are stored in your home directory and desktop as Uknown_Host.png, which keep tracks of who was trying to unlock your terminal. You can delete them at later, if you like.

i. First, place all the scripts to the home directory

ii. Create a data-base. Run 'python acc_control.py open'. It creates p.db file in your home dir. Dont remove this file ever. IF you some how delete this then you need to create a new one.

iii. Insert User Information. Run 'python acc_control.py insert' and follow the instructions

iv. If you want to add another user account then again repeat step (iii)

v. Test run, Run 'python acc_control.py passcode' and give it user name and password that you have just created.

vi. Update: If you think you need to update any information (name, user account etc) then run 'python acc_control.py update' and follow the instructions. you might need a personal "key", default is 00000, you can change it any time (line 37 and 65 of acc_control.py).

vii. Delete: run 'python acc_control.py delete', and follow the instructions

viii. Display: If you want to read the data-base of your accounts, run 'python acc_control display' and follow the instructions

ix. After creating and inserting the user account to data base file (p.db, after completing steps i to iii), edit your '.bashrc or .bash_profile' file at home dir and add a line 'python acc_control passcode' at the end.

x. Close the terminal and open again, you are supposed to see the password window. Type your password and enjoy.

xi. Note: There is also a "Back Door", in case, you completely forget your password (line 36 at passcode.py). 


Caution: It takes a snap after three consecutive faliure while providing an user name and password. The taken snaps are stored in your home directory and desktop as Uknown_Host.png, which keep tracks who was trying to unlock your terminal. You can delete them at later, if you like.
