# ST-PROJECT
 
**SOFTWARE TESTING PROJECT
System reliability testing using Chaos Engineering**
 
 
**Contents**
INTRODUCTION: -	2
1.	Creating a Hypothesis	2
2.	Identify Variables and Anticipate Effects	2
3.	Initiate the Experiment	2
4.	Measure the Impact	2
ADVANATGES & DISADVANTAGES OF CHAOS TESTING	3
CHAOS ENGINEERING TOOLS	3
•	Chaos Kong	3
•	Conformity Monkey	3
•	Chaos Gorilla	3
•	Chaos Monkey	3
CONCLUSION	4













**INTRODUCTION: -**
Chaos Testing or Chaos Engineering refers to the deliberate act of injecting failures into the system in a controlled manner in order to test the system’s ability to respond to the failure. This is a good technique to evaluate the reliability of a system by spotting errors in a specific environment so that we know already how the system would react if an unplanned failure happens in future. This technique is basically used to provide user with a better experience by testing beforehand the reaction of the system in unplanned downtime.
The practice of chaos engineering originated with Netflix around 2008 after they had formally launched their streaming service. Following a database corruption issue around 2011, Netflix planned to transition their datacenter to the cloud via AWS (Amazon Web Services). In fact, it took them eight years to finally complete the migration. In 2015, AWS experienced an outage, which caused Netflix to go down for several hours. These were the early days of cloud computing, so it was not as robust, stable, and fail-safe as it is now. When they discovered that the move to the cloud did not create some of the benefits they expected, like scalability, uptime, avoiding single points of failure, autoscaling, etc., they decided they needed a way to test for these unexpected issues to ensure their services are up and running, and ultimately, avoiding the impact to users and causing frustration. From this experience, chaos engineering was born.
There are some principles on which chaos engineering works. The general guidelines for chaos experiments are given below: -
**1.	Creating a Hypothesis**
This part contains general assumptions that how the system would react in different situations when unstable conditions are introduced as compared to normal conditions.
**2.	Identify Variables and Anticipate Effects**
In this step the experimenter needs to think by linking the testing with real life scenarios such as what will happen if very high traffic comes to your system? How will the system respond? What effect will it have on your system?
**3.	Initiate the Experiment**
Ideally everyone wants to conduct all the tests in a live environment but its necessary to have some control over the environment if the things go wrong. This is also known as controlling the blast radius. These experiments give better results when they are automated as compared to manual testing. However, there is another method in which all experiments are done in a full-fledge testing environment but obviously this would not give hundred percent true results as real-world scenarios.
**4.	Measure the Impact**
In this step we check whether the experiments give result according to our hypothesis or not. This helps us to understand whether the experiment was too limited or does it need to be scaled up in order to identify all the errors correctly. This step also helps to get more information about other errors that were skipped in previous steps.
**ADVANATGES & DISADVANTAGES OF CHAOS TESTING**
The advantages of chaos testing are:
o	IT and DevOps teams are able to more quickly identify and resolve issues that might not be captured with other testing.
o	Unplanned downtime and outages are far less likely to occur due to proactive and constant testing.
o	Strengthens system integrity.
o	Great for large, complex systems (i.e. cloud-based applications and services) as well as for scaling up

The disadvantages are:
o	Smaller systems or desktop software.
o	Applications and services that are not mission-critical to the success of the business.
o	Application environments that don’t require 24×7 uptime via customer SLAs.
o	Systems in which failures are acceptable if resolved by the end of the day.


**CHAOS ENGINEERING TOOLS**
The tools that are used in chaos engineering help the companies to allow the customers get a better experience on their site. Some of the tools used in chaos engineering are: -
**•	Chaos Kong**
This tool was designed to check that how the system would respond if a complete AWS region is dropped or deleted. Will the system be able to recover and respond by moving traffic to a different region without degrading the performance?
**•	Conformity Monkey**
Conformity Monkey is a service that runs in AWS with the purpose of identifying instances that were not conforming to predefined rules. Any instance that does not conform to the rules, which were flexible enough to be customized and set to run at different frequencies, were identified and an email notification is sent to the owner or group. Conformity Monkey has since been moved to Spinnaker services.
**•	Chaos Gorilla**
Chaos Gorilla is same as chaos monkey but on a larger scale. Chaos gorilla simulated failure on an entire AWS zone. This tool was invented to show how a large-scale disaster affected users in different regions.
**•	Chaos Monkey**
Actually, Netflix was the first site that faced the issues and due to these issues, they introduced chaos monkeys to help meet the need of continuous testing. The chaos monkeys were deployed into the system to introduce specific issues such as network delays, instances, missing data segments, etc. and simulate different real-world scenarios. Each chaos monkey had its own name and job, including:
o	Latency Monkey: Includes artificial delays
o	Conformity and Security Monkey: Hunt and kill instances that don’t adhere to best practices
o	Janitor Monkey: Cleans up and removes unused resources
o	Chaos Gorilla: Simulates an entire Amazon availability zone outage 

**CONCLUSION**
As a conclusion, it can be said that chaos engineering has grown as a separate industry in the market. There are many tools available in market that are for specific purpose of doing chaos testing such as chaos kong, conformity monkey, chaos gorilla, gremlin, chaos mesh etc. The systems are becoming complex day by day so finding and fixing errors is difficult also now. The requirements and the expectations of the users are increasing day by day so in order to provide user with an error free experience chaos engineering is the best solution as it allows the system owner to test the responses of the system on different unplanned events. At the end, I would say that chaos engineering is a good method to test the system resilience on how the system would react in case of any unplanned failure.

**REFERENCES**
Blomberg, B. (2022) Chaos engineering: Principles, examples & tools, LoadView. Available at: https://www.loadview-testing.com/blog/chaos-engineering-principles-examples-tools/ (Accessed: December 13, 2022). 
What is chaos testing? (2021) PagerDuty. Available at: https://www.pagerduty.com/resources/learn/what-is-chaos-testing/ (Accessed: December 13, 2022). 


