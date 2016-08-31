# One-Liners


Finds all of the responding targets using arp responses and then saves them to a file on the desktop.
'''

netdiscover -r 10.172.2.0/24 -P | awk 'NR<=3 { next } {print $1}' | head -n -2 >> ~/Desktop/results.txt

'''
