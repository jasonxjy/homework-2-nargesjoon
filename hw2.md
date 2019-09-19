

echo "*** Converting between the different temperature scales ***"
echo " Convert temperature from degrees Fahrenheit to degrees Celcius" 
echo "Enter temperature (C) : " read tf 
# formula (Tf-32)*(5/9)=Tc 
tc=$(echo "scale=2;(5/9) * ($tf-32)" |bc) 

KC =$(echo "scale=2;(5/9) * ($tf-32)+273" |bc)

echo "$tc C = $tf F"
echo "$KC K = $tf F"


