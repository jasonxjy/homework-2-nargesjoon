lalalalalaalal


Exercise 1

echo "*** Converting between the different temperature scales ***"
echo " Convert temperature from degrees Fahrenheit to degrees Celcius" 
echo "Enter temperature (C) : " read tf 
# formula (Tf-32)*(5/9)=Tc 
tc=$(echo "scale=2;(5/9) * ($tf-32)" |bc) 
echo "$tc C = $tf F"

Exercise 2

ls -l | grep -v ^d | wc -l

FILECOUNT="$(find . -type f -maxdepth 1 -printf x | wc -c)"

DIRCOUNT="$(find . -type d -maxdepth 1 -printf x | wc -c)"
