# ab_tests
**Part 1**

During the testing of a hypothesis for an online school, the target group was offered a new payment mechanism on the website, while the control group retained the standard payment mechanism.

**Project Goals:**

- Analyze the results of the experiment
- Define the metrics to be used in the analysis
- Determine if the differences are statistically significant
- Conclude whether the new payment mechanism should be implemented for all users

**Input Data:**

- `groups.csv` - file with information about user assignment to the control or experimental group (A – control, B – target group)
- `groups_add.csv` - additional file with users sent two days after the initial data transfer
- `active_studs.csv` - file with information about users who accessed the platform during the experiment
- `checks.csv` - file with information on user payments during the experiment

**Part 2**

Courses consist of lessons, each containing multiple tasks. We need to write an optimized query (using ClickHouse in this case) to retrieve information on the number of highly diligent students (those who completed more than 20 tasks in the current month). 

After conducting the experiment, which tested a new payment screen, we need to extract the following information on user groups in a single query:

- ARPU (Average Revenue Per User)
- ARPAU (Average Revenue Per Active User)
- Conversion Rate (CR) to purchase
- CR of active users to purchase
- CR of users active in mathematics (subject = 'math') to purchase a math course

An active user is defined as someone who has correctly solved more than 10 tasks across any subjects. A user active in mathematics is defined as someone who has correctly solved two or more tasks in mathematics over time.
