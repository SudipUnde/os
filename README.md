ls
ls -l
ls --help
clear
history
history 10
nano Mada.sh // to enter in file
#!/bin/bash  // first line in file
echo "Madan HI"
ctrl + O ; enter 
ctrl + x ; save and exit
./Madan.sh //to open file and read
but if permission is not there to open file access denied
chmod 777 Madan.sh // then
./Madan.sh // file will open 
 

Create another file 
to take input data from user
read -p "Message" data
echo "Entered data is $data"

then ctrl + o //save 
then ctrl + x // save and exit

cat filename // cat GarryBhai.sh 
will give all the commands written inside the file
 
//Addtion of two variables
read -p "Enter the number1" num1
read -p "Enter the number2" num2
echo "Addtion is $((num1 + num2))"
ctrl + o // enter
ctrl + x // save and exit 

to run // ./GarryBhai.sh


//Checking NUmber equality using -eq and if else
read -p "Enter the number" num1
read -p "Enter the number" num2

if [ $num1 -eq $num2 ]
then 
echo "True -> numbers are equal"
else
echo " False -> numbers are not equal"
fi

/////////////////////////////For loop////////////////////////////
//PRinting number using FOR LOOP
for i in {1..10}
do 
echo $i
done

ctrl+o + enter // save
ctrl + x // exit


/////////////while/////////////////////// ////////////////////////
#!/bin/bash
 
while :
do
	read -p "Enter two numnbers ( - 1 to quit ) : " a b
	if [ $a -eq -1 ]
	then
		break
	fi
	ans=$(( a + b ))
	echo "$ans"
done
////////////////////////////case//////////////////////////////////

#!/bin/bash

# Introduction
echo "Welcome to the Color Selection Program!"
echo "Which color do you like best?"

# Display color options
echo "1 - Blue"
echo "2 - Red"
echo "3 - Yellow"
echo "4 - Green"
echo "5 - Orange"

# Read user input
read -p "Enter the number corresponding to your favorite color: " color

# Process user input using a case statement
case $color in
  1) echo "Blue is a primary color.";;
  2) echo "Red is a primary color.";;
  3) echo "Yellow is a primary color.";;
  4) echo "Green is a secondary color.";;
  5) echo "Orange is a secondary color.";;
  *) echo "This color is not available. Please choose a different one.";; 
esac


/////////////////////////////////////Function/////////////////////////////

function addNumber {
a=10
b=20

# Calculate sum
sum=$(( $a + $b ))

# Display the result
echo "Sum is: $sum"
}
addNumber
