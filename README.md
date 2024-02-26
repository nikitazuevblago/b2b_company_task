# b2b_company_task
Here I've completed techincal task from "b2b-center"

A more complete and clear description is available in the .ipynb file (Jupyter Notebook)


Task class:
Customer churn
Task:
Determine the probability of churn for each customer.
The client paid us the tariff this quarter. What is the probability that he will pay us the tariff in the next quarter?



Data:

The file train_action_df.csv contains information about the most important actions on our site over the past 2 years.

fields:
     user_id - unique client identifier
     action_type - 5 types of the most important actions on our site. Categorical variable (action_4 is NOT necessarily more important than action_3, etc.)
     action_date - date of action
     cnt_actions - the number of actions of this type performed on this date


The file train_pay_df contains information about payments for the last 2 years.

fields:
     user_id - unique client identifier
     pay_date - date of payment (does NOT always correspond to the paid period!!!)
     year - year of tariff validity
     quarter - quarter of tariff validity
     tariff - impersonal tariff type
    

A few clarifications.
Quite often, clients pay the tariff in advance. For example, on November 1, 2022, they can pay for the 1st quarter of 2023.


the test_df.csv file contains clients for which you need to make a forecast


as a result, it is enough to send a file with 2 columns (user_id, proba) for all clients from the test_df.csv file