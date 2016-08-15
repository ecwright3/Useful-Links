# One-Liners


'''
netdiscover -r 10.172.2.0/24 -P | awk 'NR<=3 { next } {print $1}'
'''
