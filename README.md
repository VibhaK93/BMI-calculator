# BMI-calculator
The Body Mass Index (BMI) Calculator can be used to calculate BMI value and corresponding weight status while considering age. 

Reference: https://www.calculator.net/bmi-calculator.html?cage=31&csex=f&cheightfeet=5&cheightinch=4&cpound=160&cheightmeter=159&ckg=80&printit=0&ctype=metric&x=Calculate

{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "b75f35aa-91ff-4547-93f3-e342a2f08413",
   "metadata": {},
   "outputs": [],
   "source": [
    "BMI Calculator\n",
    "\n",
    "# For Reference: \n",
    "\n",
    "#BMI = (weight x 703) / (height  x height )"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 48,
   "id": "5e412e65-b677-467c-824e-3d3adc51bab2",
   "metadata": {},
   "outputs": [],
   "source": [
    "# For Reference\n",
    "\n",
    "Classification\tBMI range - kg/m2\n",
    "Severe Thinness\t< 16\n",
    "Moderate Thinness\t16 - 17\n",
    "Mild Thinness\t17 - 18.5\n",
    "Normal\t18.5 - 25\n",
    "Overweight\t25 - 30\n",
    "Obese Class I\t30 - 35\n",
    "Obese Class II\t35 - 40\n",
    "Obese Class III\t> 40"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "6c4b2f69-f9c0-44cc-af19-88b41cd24407",
   "metadata": {},
   "outputs": [],
   "source": [
    "\n",
    "name = input(\"Enter your name: \")\n",
    "\n",
    "age = input(\"Enter your age (age should be between 2 - 100) \")\n",
    "\n",
    "gender = input(\"Enter you gender: \")\n",
    "\n",
    "weight = int(input(\"Enter your weight in pounds: \"))\n",
    "\n",
    "height = int(input(\"Enter your height in inches: \"))\n",
    "\n",
    "BMI = (weight * 703) / (height * height)\n",
    "\n",
    "print(BMI)\n",
    "\n",
    "if BMI>0:\n",
    "    if(BMI<16):\n",
    "        print(name +\", you have severe thinness.\")\n",
    "    elif (BMI<=17):\n",
    "        print(name +\", you have moderate thinness.\")\n",
    "    elif (BMI<=18.5):\n",
    "        print(name +\", you have mild thinness.\")\n",
    "    elif (BMI<=25):\n",
    "        print(name +\", you are normal.\")\n",
    "    elif (BMI<=30):\n",
    "        print(name +\", you are overweight, you may benefit from more exercise.\")\n",
    "    elif (BMI<=35):\n",
    "        print(name +\", you are in obese Class I, you may benefit from more exercise.\")\n",
    "    elif (BMI<=40):\n",
    "        print(name +\", you are in obese Class II, you may benefit from more exercise.\")\n",
    "    else:\n",
    "        print(name +\", you are in obese Class III, you may benefit from more exercise.\")\n",
    "else:\n",
    "    print(\"Enter valid input\")\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "13ad9c6e-e489-4c25-87a5-2811e44ce57f",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python [conda env:base] *",
   "language": "python",
   "name": "conda-base-py"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.12.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
