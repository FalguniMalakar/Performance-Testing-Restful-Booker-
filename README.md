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

![0](https://github.com/FalguniMalakar/Performance-Testing-Restful-Booker-/assets/153453822/e48f7605-7c3a-4a32-95fc-5e61c9865bac)

**Load Testing:**
For finding the maximum load capacity of restful-booker.herokuapp.com when reqesting a collection of API, Jmeter is used where Thread Groups of huge number of threads(users) are made. For this test, Thread Groups of 100, 300, 600 and 1200 threads are found to be suitable data. For all Thread Groups, Ramp-up period is set to 10s with loop count of 1.
![1](https://github.com/FalguniMalakar/Performance-Testing-Restful-Booker-/assets/153453822/e3f26b69-3e85-4f77-98e1-0808d92503db)


**Run the JMeter test for each scenario using the following command:**
Using the command-line interface, the following command-line is used for making JTL files where we can see the load testing results in command-line interface.
![Capture](https://github.com/FalguniMalakar/Performance-Testing-Restful-Booker-/assets/153453822/4c568fad-20d9-4f6e-b40a-9c123a6b7e07)

**View Result Tree:**
Provides detailed information on each request and response, allowing for in-depth analysis of individual transactions.
![2](https://github.com/FalguniMalakar/Performance-Testing-Restful-Booker-/assets/153453822/e8301d69-5de4-400a-b433-1f266f995fb2)

**Summary Report:**
Summarizes key performance indicators such as average response time, throughput, and error rates.
![3](https://github.com/FalguniMalakar/Performance-Testing-Restful-Booker-/assets/153453822/5e97de23-ef62-4007-a512-0aff6fc39f41)

**Aggregate Report:**
Aggregates data from multiple samples to give an overview of the entire test run, including minimum, maximum, and average values.
![4](https://github.com/FalguniMalakar/Performance-Testing-Restful-Booker-/assets/153453822/4af77724-5331-4175-bfb8-1da0ff46a9ea)

**Backend Listener:**
Collects and forwards metrics to external systems for further analysis, integrating JMeter with external monitoring tools.
![5](https://github.com/FalguniMalakar/Performance-Testing-Restful-Booker-/assets/153453822/87da568b-dde6-414f-9c46-f248e87d2432)

**Results Analysis:**
Based on the generated reports, we conducted a thorough analysis of the performance under varying load conditions.
![6](https://github.com/FalguniMalakar/Performance-Testing-Restful-Booker-/assets/153453822/58aea269-09d8-4a34-97b1-7cfcd291d7d5)

**Throughput Chart:**
The throughput chart visualizes the number of requests processed by the website per unit of time. A higher throughput indicates better performance in handling user requests.
![7](https://github.com/FalguniMalakar/Performance-Testing-Restful-Booker-/assets/153453822/d0706f55-66be-44fb-8a6c-30697ead468a)
**Conclusion:**
Therefore from this in-depth performance testing of restful-booker.herokuapp.com for a collection of API using Thread Groups, it is determined that the maximum load capacity of running the aforementioned collection of APIs without any errors is 5500 concurrent threads and with very minor errors (less than 1%) is 5500 concurrent threads. Using threads any more than this causes significant amount of errors.
