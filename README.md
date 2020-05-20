# CyPass

This is an aggressor-script used to bypass Cylance's memory exploitation defense library. It utilizes the research found [here](https://dru1d.ninja/2018/11/02/Cylance-Bypass/), to diable the library and dump lsass using procdump. The script also uses a random number generator to select one of four diffrent names of procdump to upload to the specified machine (for added stealth). Besides the need of having a system level beacon, you need to do the following for this script to run as intended: 
- wait for client call backs (beacon check-ins) before executing other stages of the script
- excute this script on one host at a time 
