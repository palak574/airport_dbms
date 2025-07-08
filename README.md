✈️ Airport Database Management System
This project is a comprehensive relational database solution to manage and analyze airport operations data.
It includes 20 SQL problem statements covering various business questions related to flights, passengers, and airports.

📂 Project Overview
The Airport Database Management System uses MySQL to store and analyze data about:

Flights

Passengers

Seat utilization

Distances between cities

Year-over-year growth metrics

The project demonstrates proficiency in:

✅ SQL query design
✅ Window functions
✅ Aggregation and grouping
✅ Analytical functions (LAG, LEAD)
✅ Data transformation

🛢️ Database Used
Database Name: airport_db
Primary Table: airports2

Example table columns:

Origin_airport

Destination_airport

Origin_city

Destination_city

Passengers

Seats

Flights

Distance

Fly_date

📝 Problem Statements Solved
Below is a summary of the 20 problems addressed:

1️⃣ Retrieve all tables in the database.
2️⃣ Display the first 5 rows of the airports2 table.
3️⃣ Aggregate total passengers by origin and destination airports.
4️⃣ Calculate average seat utilization between airports.
5️⃣ Generate year-wise passenger totals for each route.
6️⃣ Compute year-over-year passenger growth with LAG.
7️⃣ Identify declining passenger trends across years.
8️⃣ Count total flights per route per year.
9️⃣ Compute year-over-year flight growth.
🔟 Calculate growth indicators for flights (increasing vs decreasing).
1️⃣1️⃣ Aggregate total passengers per month per city.
1️⃣2️⃣ Identify peak passenger month for each origin city.
1️⃣3️⃣ Retrieve months with highest passenger volumes.
1️⃣4️⃣ Calculate the average flight distance between each city pair.
1️⃣5️⃣ Rank the city pairs by average distance traveled.
1️⃣6️⃣ Identify the top 5 routes with the largest passenger declines.
1️⃣7️⃣ Generate summary statistics for sales, seats, and utilization.
1️⃣8️⃣ Filter flights where seat utilization exceeds a given threshold.
1️⃣9️⃣ Rank flights by passenger volume per year.
2️⃣0️⃣ Generate a report combining flight counts and passenger counts per route.

💻 Technologies Used
Database: MySQL

Python Libraries:

SQLAlchemy (for connection)

Pandas (data manipulation)

Visualization:

Plotly Dash (optional dashboards)

🛠️ Setup Instructions
Install MySQL and create the airport_db database.

Load the airports2 table with your data.

Install required Python libraries:

bash
Copy
Edit
pip install sqlalchemy pandas plotly dash pymysql
Update the database credentials in your Python scripts.

Run your queries or dashboards.

📊 Example Query
Retrieve total passengers grouped by airport:

sql
Copy
Edit
SELECT 
  Origin_airport, 
  Destination_airport, 
  SUM(Passengers) AS total_passengers
FROM airports2
GROUP BY 
  Origin_airport, 
  Destination_airport
ORDER BY 
  total_passengers DESC;
🌟 Outcomes
This project demonstrates:

✅ Advanced SQL querying skills
✅ Proficiency in data aggregation, window functions, and reporting
✅ Ability to translate business questions into SQL solutions
✅ Use of Python for database connectivity and dashboards

📧 Contact
If you have any questions, feel free to reach out!
