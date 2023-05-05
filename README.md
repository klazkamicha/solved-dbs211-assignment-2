Download Link: https://assignmentchef.com/product/solved-dbs211-assignment-2
<br>
In this assignment, you create a simple HR application using the C++ programming language and Oracle server. This assignment helps students learn a basic understanding of application development using C++ programming and an Oracle database.

<strong>Instruction:</strong>

In this assignment, we complete the application from the first part to insert, update, and delete the employee information.

You need to implement the following functions:




<strong><em>void insertEmployee(*conn,  struct Employee emp);</em></strong>




This function receives a connection pointer and a structure of type Employee and inserts the given employee information stored in the parameter <strong><em>emp</em></strong> to employee table.

In function <strong><em>insertEmployee()</em></strong>, call the function <strong><em>findEmployee()</em></strong> to see if the employee number of the given employee exists. If an employee with the same employee number exists display a proper message:

“An employee with the same employee number exists.” and return to the menu.

Otherwise, insert the employee information into the employee table and display the following message:

“The new employee is added successfully.”




<strong><u>Note</u></strong>: For simplicity, assume that the office code of the new employees is 1 and the manager id (reportsTo) is 102 by default.




<strong><em>void updateEmployee(*conn,  int employeeNumber);</em></strong>This function receives a connection pointer and an integer number as the employee number and updates the phone extension for the given employee. In function <strong><em>updateEmployee()</em></strong>, call function <strong><em>findEmployee() </em></strong>to see if the employee exists in table employees. If employee does exist, ask the user to enter the new phone extension. Store the new extension in table employees for the given employee number.




<strong><em>void deleteEmployee(*conn,  int employeeNumber);</em></strong>

This function receives a connection pointer  and an integer number as the employee number and deletes a row with the given employee number from table employees. In function <strong><em>deleteEmployee()</em></strong>, call function <strong><em>findEmployee()</em></strong> to see if the employee with the given employee number exists. If the employee does not exist display a proper message:

“The employee does not exist.”

If the employee exits, delete the row from table employees and display a proper message:

“The employee is deleted.”

<strong>Function <em>main()</em></strong>

From the menu in the first part of the assignment, complete options 3 to 5.




<ul>

 <li>Find Employee</li>

 <li>Employees Report</li>

 <li>Add Employee</li>

 <li>Update Employee</li>

 <li>Remove Employee</li>

 <li>Exit</li>

</ul>

<strong>Add an Employee</strong>

If the user chooses option 3, prompt the user to enter the new employee information and store them into a variable of type Employee structure. Then, call function <strong><em>insertEmployee()</em></strong> to insert the new employee information in table employees.

<strong>Employee Number: 1818Last Name: AdamFirst Name: SarahEmail: </strong><a href="/cdn-cgi/l/email-protection#85f6e4e1e4e8c5e0e8e4ece9abe6eae8"><strong><span class="__cf_email__" data-cfemail="146775707579547179757d783a777b79">[email protected]</span></strong></a><strong>extension: x4411Job Title: Sales RepCity: Toronto</strong>

<strong>NOTE:</strong> You do not need to ask the user to enter values for the members <em>reportsTo</em> and <em>phone</em>.

<strong>Update an Employee</strong>

If the user chooses option 4, ask the user to enter the employee number:

Employee Number: 1216

Then, call function <strong><em>updateEmployee()</em></strong> to update the phone extension for the row with the employee number <strong>1216</strong>. In this function, the user is asked to enter the new extension:

New Extension: x2111

The extension column of the row with the employee number 1216 will be updated with the new value x2111.

<strong>Delete an Employee</strong>

If the user chooses option 5, ask the user to enter the employee number:

Employee Number: 1818

Then, call function <strong><em>deleteEmployee()</em></strong> to remove the employee from table employees.

<strong><u>Note</u></strong>: For each query in your assignment, make sure you handle the errors and display the proper message including the error_code.

Error_code is a number returned if the query execution is not successful.