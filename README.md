# bmi_calculator
Software development 1 - Coursework 1 - Stany Vanhemelrijck

This program was created in Oktober 2021 as my first coursework for my Software and Development class. 
The program gives a choice between the metric and imperial measurement systems. After that, it asks for two inputs, one height and another weight. It then asks for confirmation from the user that the correct input is given. It then returns the BMI value and category determined by the WHO.


PSEUDOCODE: 

    PRINT title (Body Mass Index Calculator) + welcome message

    To the variable choice we assign an INPUT (Which system of measurement would you like to use? Type METRIC (kg & m) for the metric system or IMPERIAL (lb & foot)     for the imperial system and press ENTER.)

    Imperial system: 
    IF choice is equal to ‘imperial’ THEN
        ask for an INPUT (enter your weight in pounds) and assign it to variable imperial_weight
        ask for an INPUT (enter your height in inches) and assign it to variable imperial_height
        PRINT out the information back to the user.

        ask the user if the input is correct INPUT (Check if your answers are correct. Type YES if you want to continue or type NO if you would like to alter your answers and press ENTER)

        IF the user inputs ‘yes’ THEN
            perform the bmi calculation and assign it to variable imperial_BMI Weight(lb) / height^2(inches) *703
        IF the user inputs ‘no’ THEN ask input again (loop)
        PRINT the result, imperial_BMI
    
    IF imperial_bmi is smaller than (< ) 18.5 THEN 
        PRINT (you are underweight)
    IF imperial_bmi is bigger or equal to (>=) 25 THEN 
        PRINT (you are overweight)
    IF imperial_bmi is bigger than (>) 30 THEN 
        PRINT (you are obese)
    In any other case
        PRINT (you are normal)
    
    Metric system:
    IF choice is equal to ‘metric’ THEN
        ask for an INPUT (enter your weight in kilograms) and assign it to variable metric_weight
        ask for an INPUT (enter your height in meters) and assign it to variable metric_height
        PRINT out the information back to the user.

        ask the user if the input is correct INPUT (Check if your answers are correct. Type YES if you want to continue or type NO if you would like to alter your answers and press ENTER)
    
        IF the user inputs ‘yes’ THEN
            perform the bmi calculation and assign it to variable metric_BMI. Weight(kg) / height^2(m)
        IF the user inputs ‘no’ THEN 
            ask input again (loop)
        PRINT the result, metric_BMI
    
    IF metric_bmi is smaller than (< ) 18.5 THEN 
        PRINT (you are underweight)
    IF metric_bmi is bigger or equal to (>=) 25 THEN 
        PRINT (you are overweight)
    IF metric_bmi is bigger than (>) 30 THEN 
        PRINT (you are obese)
    In any other case
        PRINT (you are normal)
   
    
