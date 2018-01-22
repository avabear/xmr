android rooted 5.0+ xmrig miner

This will work on Android 32/64bit ARM processors and some Intel Junk.
You'll need a terminal apk called TERMUX from f-droid.
F-DROID is a kind of 'g00gleplay' but without all of the ADS and BS. Thank God.
Also included below is a GREAT keyboard apk. You'll like the keyboard, seriously.


https://f-droid.org/repo/com.termux_59.apk          <--TERMUX Terminal
https://f-droid.org/repo/org.pocketworkstation.pckeyboard_1039003.apk <-- keyboard

install and open termux (and the keyboard if you'd like to make your life easier)

First thing!! Click `Aquire Wakelock` from the notification drop down.
Or just type in the command(termux-wake-lock)in the list of commands below.

You'll see a '$' This is your terminal. You type commands into it lol.

'ls' lists files
'cd' changes directory
'./' runs a program (./xmrig)
'exit' then enter enter shuts it down

The best thing to do is to fork this rep and edit yourconfig.json file
BEFORE you install it on your phone or chromebook
so that you don't need to use nano!!
CHANGE THE ETN WALLET ADDRESS



TYPE these commands into your terminal

termux-wake-lock											(keep Termux running after screen sleeps)

apt update													(gets a list of apps)

apt upgrade -y												(update the list of apps)

apt install git libuv-dev -y								(install apps we need so we can mine)

git clone https://github.com/mystapler/miners.git			(this installs the miners in a file called 'miners')

NOW, EVERYTHING IS INSTALLED IN A FILE CALLED 'miners'


Setting up your config.json file with NANO text editor thats built into your terminal!!

nano ~/miners/android_arm86/config.json


(Here's why you're going to want that special keyboard...)

This is where things get a little shitty for anyone new to the nano text editor.
There are only three fields you will (probably) need to change to get started.
These are the `threads`, `url`, and `user` fields.
Everything else can be left the same.

`threads`:	Number of threads. 
`url`:		Pool Address.
`user`:		Pool Username. Mine is 'x'



To move the cursor on regular keyboard


Volume Up + W,A,S,D; this is to go up, left, down, and right respectively.


Then, once the file has been edited, press

Volume Down + X to "save and exit". Hit y to confirm the save, and then push enter!

JESUS CHRIST!
The file should be saved at this point! You should be ready to mine!

#RUN THE MINER#
Get on your terminal and find the miners file and you specific type of processor.
86 for old stuff and 64 for new stuff.
My (oneplus one) phone uses a 32bit proc so I choose arm86!!

Enter these commands to start mining...


cd miners													(change dir to miners)

cd android_arm86										(change dir to miner you need)

./xmrig														(runs the miner and ctrl-c stops it)



Have Fun!!
