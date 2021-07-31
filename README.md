# CarPwner

CarPwner is a python script to "jam", capture, and replay rolling code signals using two yard stick one devices and rfcat.

This is done by jamming the receiver, capturing two or more remote presses, then stopping the jammer and replaying the first remote press saving the next capture in the rolling code series to replay later.

This script simply combines everything into a single script that automates the process. It is up to you to follow all of the laws in your area. Jamming a signal is not legal in many areas. 
The author(s) of this code take no responsibility for your use or misuse of the script. 
Please follow all local, state, federal, and international, and religious laws.


Capture and replay first code automatically: python CarPwner.py -f 315060000 -r 1818 -m -40 -o -2500000 -O capture.io
Capture and wait for keypress to replay first code: python CarPwner.py -f 315060000 -r 1818 -m -40 -o -2500000 -O capture.io -k
Load previous captures to replay: python CarPwner.py -I capture.io
