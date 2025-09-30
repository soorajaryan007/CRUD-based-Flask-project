Practice Exercises
The following are some practice exercises for the interested learners. We are not providing the solutions for these exercises to encourage the learners to try them on their own. Please feel free to use the course discussion forum for sharing your opinions on the solution with other interested learners.

Exercise 1: Search Transactions
In this exercise, you will add a new feature to the application that allows users to search for transactions within a specified amount range. You will create a new route called /search that handles both GET and POST requests in app.py.
Correct code reference

Instructions:

Create a new function named search_transactions and use the @app.route decorator to map it to the URL /search.

Inside the function, check if the request method is POST. If it is, retrieve the minimum and maximum amount values from the form data submitted by the user. Convert these values to floating-point numbers.

Filter the transactions list based on the amount range specified by the user. Create a new list, filtered_transactions, that contains only the transactions whose amount falls within the specified range. You can use a list comprehension for this.

Pass the filtered_transactions list to the transactions.html template using the render_template function. In this template, display the transactions similar to the existing transactions.html template.

If the request method is GET, render a new template called search.html. This template should contain a form that allows users to input the minimum and maximum amount values for the search.

Exercise 2: Total Balance
In this exercise, you will add a new feature that calculates and displays the total balance of all transactions. You will create the route in app.py.
Correct code reference

Instructions:

Create a new function named total_balance and use the @app.route decorator to map it to the URL /balance.

Inside the function, calculate the total balance by summing the amount values of all transactions in the transactions list.

Return the total balance as a string in the format “Total Balance: {balance}”.

To display the total balance, you do not need to create a new template. Instead, you will modify the transactions.html template to include the total balance value at the bottom of the table.

After displaying the list of transactions in the transactions.html template, add a new row to display the total balance. You can use the same render_template function as before, passing both the transactions list and the total balance value.


