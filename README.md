# Performance-Testing-Restful-Booker
**Overview:**
Hello and welcome! This GitHub repository contains the performance testing documentation for restful-booker.herokuapp.com, for a collection of API with various HTTP methods. Here, performance testing is done using Jmeter to determine the maximum load capacity of this collection of API to be called without any errors when a huge number of concurrent threads(users) are made.

All the test files (jmx, jtl & html files) are included in this repository and the following is a report of all the test procedures and reports.

**Tools Used:**
Apache JMeter: A powerful open-source tool for performance testing, capable of simulating heavy loads on servers and analyzing the overall performance of web applications.
JMeter Plugins: Additional plugins used to enhance JMeter's capabilities.

**Listeners Used:**
View Result Tree,
Summary Report,
Aggregate Report,
Backend Listener.

**Test Scenarios:**
We created multiple test scenarios with varying numbers of concurrent users to simulate real-world usage patterns.

**Collection of API:**
A set of API for restful-booker.herokuapp.com covering various HTTP methods i.e. POST, GET, DELETE, and PUT are used for test data. Data is set, called, then updated using token and then deleted using token all within this set of API for this test coverage.


**Load Testing:**
For finding the maximum load capacity of restful-booker.herokuapp.com when reqesting a collection of API, Jmeter is used where Thread Groups of huge number of threads(users) are made. For this test, Thread Groups of 100, 300, 600 and 1200 threads are found to be suitable data. For all Thread Groups, Ramp-up period is set to 10s with loop count of 1.

**Run the JMeter test for each scenario using the following command:**
Using the command-line interface, the following command-line is used for making JTL files where we can see the load testing results in command-line interface.

**View Result Tree:**
Provides detailed information on each request and response, allowing for in-depth analysis of individual transactions.

**Summary Report:**
Summarizes key performance indicators such as average response time, throughput, and error rates.

**Aggregate Report:**
Aggregates data from multiple samples to give an overview of the entire test run, including minimum, maximum, and average values.

**Backend Listener:**
Collects and forwards metrics to external systems for further analysis, integrating JMeter with external monitoring tools.

**Results Analysis:**
Based on the generated reports, we conducted a thorough analysis of the performance under varying load conditions.

**Throughput Chart:**
The throughput chart visualizes the number of requests processed by the website per unit of time. A higher throughput indicates better performance in handling user requests.

**Conclusion:**
Therefore from this in-depth performance testing of restful-booker.herokuapp.com for a collection of API using Thread Groups, it is determined that the maximum load capacity of running the aforementioned collection of APIs without any errors is 5500 concurrent threads and with very minor errors (less than 1%) is 5500 concurrent threads. Using threads any more than this causes significant amount of errors.
