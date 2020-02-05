# SpectumNextDevWin10Setup
Some details around my development environment for ZX Spectrum Next  

#Computer  
Macbook Pro (2013)- Retina i7, 16Gb 500Gb SSD. External 1Gb SSD Runing Windows 10 on USB  

#OS  
Windows 10 Pro (1990 at time of writing) on External SSD  

#Editor  
Sublime Text 3 with Paid License  
https://www.sublimetext.com/  

#Z80 Plug-In  
https://github.com/psbhlw/sublime-text-z80asm  


#Assembler  

https://github.com/z00m128/sjasmplus

example cmd  
..\Tools\sjasmplus --zxnext=cspect --nofakes --nologo --msg=err --sym=.\Main.sym .\Main.asm  



#Misc Tools  
##NexCreator.exe  
https://github.com/Threetwosevensixseven/NexCreator  
Used to create nex file, sjasm can do that too, but I have still to port my code.  

Example file  
BlockRacer.sna,5,4000  
!BMP8,AppyZXSplash.bmp,0,0,0,0,196  
.\spritedata\br_start.nxi,12,c000  

example cmd  
..\Tools\NexCreator.exe NexList.txt Game\BlockRacer.nex  

#Emulator  
http://dailly.blogspot.com/
Found on Mike's blog  
..\..\Tools\CSpect.exe -zxnext -tv -brk -w3 -s28 -16bit -map=..\main.smm -mmc=.\ BlockRacer.nex  


Graphics  
I work with Photoshop monthly subscription  

#Udgee-Next : Sprite editor  
https://www.specnext.com/udgee-sprite-editor/  

#NetRaw  
https://github.com/stefanbylund/zxnext_bmp_tools    
I use this to create startup screen image in raw pixel format to send to layer 2
..\..\Tools\nextraw.exe -no-palette br_start.bmp  
