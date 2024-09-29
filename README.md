# WesternGovenorsUniversity.IntroPythonD335

34.1 PRACTICE: Assign variables, mathematical operations
Instructions:
Create a Python solution to the following task. Ensure that the solution produces output in exactly the same format shown in the sample(s) below, including capitalization and whitespace.

Task:
Create a solution that accepts three integer inputs representing the number of times an employee travels to a job site. Output the total distance traveled to two decimal places given the following miles per employee commute to the job site. Output the total distance traveled to two decimal places given the following miles per employee commute to the job site:

Employee A: 15.62 miles
Employee B: 41.85 miles
Employee C: 32.67 miles
The solution output should be in the format

Distance: total_miles_traveled miles

#Employee A: 15.62 miles
#Employee B: 41.85 miles
#Employee C: 32.67 miles
#solution accepts three integer inputs representing the number of times an employee travels to the job site
#solution outputs "Distance: " followed by the total value to two decimal places

travels = {
    'A' : int(input()),
    'B' : int(input()),
    'C' : int(input())
}    

mpe = {'A': 15.62, 'B': 41.85, 'C': 32.67}

totals_miles_traveled = sum(travels[employee] * mpe[employee] for employee in travels)

print(f"Distance: {totals_miles_traveled:.2f} miles")
