![Screenshot (196)](https://user-images.githubusercontent.com/86251750/142449753-404f586c-7999-43fe-9880-33ac335e894c.png)
 An Ecommerce company based in New York City that sells clothing online but they also have in-store style and clothing advice sessions. Customers come in to the store, have sessions/meetings with a personal stylist, then they can go home and order either on a mobile app or website for the clothes they want.
 
 **OBJECTIVE**
--------------------------
The company is trying to decide whether to focus their efforts on their mobile app experience or their website. so I used various plots and then Decided to use Linear Regression as my model.

**Dataset**
---------------------------
This datset has been taken from [kaggle](https://www.kaggle.com/panditdandgule/ecommerce-customers)

**About the Dataset**
--------------------------
Here are what the columns represent:

We'll work with the Ecommerce Customers csv file from the company. It has Customer info, suchas Email, Address, and their color Avatar. Then it also has numerical value columns:

-Avg. Session Length: Average session of in-store style advice sessions.

-Time on App: Average time spent on App in minutes

-Time on Website: Average time spent on Website in minutes

-Length of Membership: How many years the customer has been a member.

Here are three common evaluation metrics for regression problems:

**Mean Absolute Error** (MAE) is the mean of the absolute value of the errors:

![Screenshot (194)](https://user-images.githubusercontent.com/86251750/142446781-acbf3f3c-7979-4c19-8d79-9d81d5e77756.png)

**Mean Squared Error** (MSE) is the mean of the squared errors:

![Screenshot (195)](https://user-images.githubusercontent.com/86251750/142446933-4c3b30c9-d342-4087-bebc-239e9a047a57.png)

**Root Mean Squared Error** (RMSE) is the square root of the mean of the squared errors:

![Screenshot (193)](https://user-images.githubusercontent.com/86251750/142447011-6d0c81dc-ba91-4375-b2a0-2b5ce23687dc.png)

Comparing these metrics:

- **MAE** is the easiest to understand, because it's the average error.
- **MSE** is more popular than MAE, because MSE "punishes" larger errors, which tends to be useful in the real world.
- **RMSE** is even more popular than MSE, because RMSE is interpretable in the "y" units.

All of these are **loss functions**, because we want to minimize them.

**Model Accuracies:**
-------------------------

| Model              | MAE                |  MSE             | RMSE              |
| -------------      |:-------------:     |:-------------:   |:-------------:    |
|  Linear Regression | 7.228148653430845  |79.81305165097471 | 8.93381506697865  |

## CONCLUSION
------------------------

Do we focus our effort on mobile app or website development? Or maybe that doesn't even really matter, and Membership Time is what is really important. Let's see if we can interpret the coefficients at all to get an idea.

![Screenshot (197)](https://user-images.githubusercontent.com/86251750/142451984-5f651693-0fdc-4b52-bfde-1cbc88f32a9d.png)

**Interpreting the coefficients:**

Holding all other features fixed, a 1 unit increase in Avg. Session Length is associated with an increase of *25.98* total dollars spent.
Holding all other features fixed, a 1 unit increase in Time on App is associated with an increase of *38.59* total dollars spent.
Holding all other features fixed, a 1 unit increase in Time on Website is associated with an increase of *0.19* total dollars spent.
Holding all other features fixed, a 1 unit increase in Length of Membership is associated with an increase of *61.27* total dollars spent.

## Final Thoughts:
----------------------

**There are two ways to think about this: Develop the Website to catch up to the performance of the mobile app, or develop the app more since that is what is working better. This sort of answer really depends on the other factors going on at the company**

***language used***
--------------------------
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

**Tools**
-----------------------
[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)    ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)   ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)   ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)  ![Made with matplotlib](https://user-images.githubusercontent.com/86251750/132984208-76ce70c7-816d-4f72-9c9f-90073a70310f.png)  ![seaborn](https://user-images.githubusercontent.com/86251750/132984253-32c04192-989f-4ebd-8c46-8ad1a194a492.png)
