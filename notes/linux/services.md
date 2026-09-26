## Day six
Today i learn't the difference between ps and top. ps lists the processes running in one terminal instance while top shows
live of what processes are curently running. if you want to know what processs use a lot of memory check the RES coloum 
Also the MEM
& this command is used to run comands  in the background so you can run other things in the same terminal 
KILL<pid> is used to kill a processes that is currently running and you get PID from PS,and TOP it shows the id of a runnining
process
four systemct1 commands are 
1)status;gives you information about process that are running
2)start; starts a process
3)stop; stops a process
4) restart; automatically starts aftter stoping a process
enabed is default meaning most services start when you installed. actice means its currently running. 
we used curl localhost beacuse we wanted to be sure if it was actually running 
##MISTAKES
i also typed systemct1 (number 1 instead of letter L) and got command not found
i got stuck inside the less pager after a long systemctl status output and didn't realize you needed to press q to exit
