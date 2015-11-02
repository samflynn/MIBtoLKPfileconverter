# MIBtoLKPfileconverter

Abbreviations Used 
SNMP : Simple Network Management Protocol
MIB : Management Information base
LKP : Look up file
FMS : Fault Management System

A Shell script to convert SNMP MIB alarm files of a telecom network to LKP configuration files that can be loaded on to a Fault management system. 

As there are no clear explicit rules that define how a MIB file is to be written, hence different network vendors define them in their own way, beacause of this these files cannot be loaded directly into a FMS for exxample NETboss.

So they need to be converted into a LKP file, that can easilt be loaded into the FMS.

This shell script can convert these MIB files into machine readable LKP files. This shell uses basic Shell fuctions like awk, grep, sed. Additional extended awk fucntions should be added to successful run script on system.

This script has be tested on 260 MIB files, total containing 2463 Traps.

Working of the code explained using a flow diagram:
http://i.imgur.com/2e47YlV.png?1

A detailed technical analysis of the code : 
https://drive.google.com/file/d/0B9P591Bk1VTgaDhYN1BaS2Y3ME0/view?usp=sharing
