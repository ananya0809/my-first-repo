files () 
{
 ls | wc -l
}
nfiles=$( files - 1 )
correct=0
digit='^[0-9]+$'
while [ $correct -ne 1 ]
do
	read -p "How many files are in the current directory: " ans
	if ! [[ $ans =~ $digit ]]
	then
		echo "Enter a Number"
	elif [ $ans -gt $nfiles ]
	then
		echo "Too High"
	elif [ $ans -lt $nfiles ]
	then
		echo "Too Low"
	else
		echo "Congratulations you guessed Correctly!"
		break
	fi
done
