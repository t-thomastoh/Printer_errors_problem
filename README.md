# Printer_errors_problem
Python practice

Task:
You have to write a function printer_error which given a string will output the error rate of the printer as a string representing a rational whose numerator is the number of errors and the denominator the length of the control string.

Solution:
normal = 'abcdefghijklm'
def printer_error(s):
    errors = 0
    count = len(s)
    for i in s:
        if i not in normal:
            errors += 1
        
    return str(errors) + "/" + str(count)  
    
s="aaaaaaaaaaaaaaaabbbbbbbbbbbbbbbbbbmmmmmmmmmmmmmmmmmmmxyz" #Use this string to create determine the number of error
printer_error(s)
