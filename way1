#!/usr/bin/bash

MYSTRING="Do something in bash"
echo $MYSTRING



#way 1

func()
{
/usr/bin/python << EOF   #issue with passing command line argument in it
import sys
print sys.argv
myPyString = "Do something on python"
print myPyString
class my(object):
	def __init__(self):
		self.x = 12
		self.y = 13

d=my()
print d.x
print d.y
import os
print os.listdir('.')

EOF


}

func "1" "2"

echo "Back to bash"


#way 2


func_two() ##passing command line are working fine
{
/usr/bin/python -c'
import os;
import sys;

def foo(x,y):
	print "Inside Function";
	print "sum",int(x)+int(y)
	#print os.listdir(".");
foo(sys.argv[1],sys.argv[2]);
' $1 $2

}
#"x" "y"

func_two 92 91




