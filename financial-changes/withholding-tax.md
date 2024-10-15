---
icon: badge-percent
---

# Withholding Tax

Withholding is deducted from prize money when PMR is foreign. It can be used in following ways

* Paid to RTO as ‘Withholding Tax Refund Check’
* Paid to IRS as ‘IRS Payment’
* Paid to Entry as ‘Account Transfer’ if it is moved to account register

### **Transfer Withholding Tax to Account Register:**

When we click on ‘TRANSFER/PAY W.H. TAX’ then a dialog will appear. This dialog will display the total withholding tax for the selected year that is neither moved to the account register nor paid to the IRS.

* **Tax Withheld:** The total withholding tax deducted from prize money for the selected year.
* **Tax Paid:** Withholding Tax that is already moved to the account register.
* **Available For Transfer:** Withholding Tax that is not moved to account register yet.

**Account Register Changes:**

When withholding tax is transferred to account register then a account register record is created with type ‘Withholding Tax Refund’

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdyUW_ZJzxdWSPeimJDPqDG_0HuJmdY_DMlUVCsI1BRQ2YDPq-S48kNhvxkhvZ5GyjoGiiOGPYbrQUPxofwWq5EHXBD70uKGkKcJAsj795ount20Tp023krOzBeTpXxHXj2q4dC2DLtdJiQVOVUTd26h7Q?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

**Example:**For RTO ‘HIDDEN RIDGE’ we have transferred $20 to the account register. Then the following account register is created.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdNyeUf_1nUB0S4qFk7CbtcmgnUli2RVGXiTozvfwEqEViB8Aob9-NujICgWXscQCFm2xD73kw-yhKAZ94wLgEfP_bt8lISK93x0pyz0kY2Ikz39YDXDZ4OoQ-_U0jQYWV6z6i_18HG0xeX3BQMXzZZPt9a?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

### **Pay Withholding Tax to RTO:**

The withholding tax that is moved to the account register can be paid to the RTO as ‘Withholding Tax Refund’ using ‘Pay to RTO’.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdeQD4wUaOqEIv-EIpe5b38oOuEzTSVO9WDRLGZjFlDpxQrszGzDbkQO8Td7FbH-s244HxDVkjvt_Inq8RJb2bmGgOUulYoikNsMEmQcf9YWBPxLu4rNvXKgTCrk9oUo2yo2tCyAF1QwnRv3VI4_cXLwe7t?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

**Account Balance Effect On Check:**

* If RTO has a debit account balance then ‘Withholding Tax Refund Check’ cannot be created.
* If RTO has a zero account balance then all the available withholding tax refund can be paid as  ‘Withholding Tax Refund Check’.
* If RTO has credit account balance then whichever is smaller account balance or withholding tax refund can be paid as ‘Withholding Tax Refund Check’. E.g account balance is -100, Withholding Tax Refund id -50 then maximum amount of which the check can be created is 50.

**Account Register Changes:**

* **Check Generated for 4D or Cloud Withholding Tax Refund:** When the check is generated from a withholding tax refund that was moved to the account register using either 4D or Cloud only, a single account register record will be created.
* **Check Generated for Combination of 4D and Cloud Withholding Tax Refund:** When the check is generated from a withholding tax refund that was moved to the account register using both 4D and Cloud, two separate account register records will be created to record the amounts paid using 4D credit and Cloud credit.



### **Withholding Payments - Quick Action:**

Withholding tax that is not moved to the account register can be paid to the IRS using RTO quick action ‘Withholding Payments’.

**Withholding Tax Batch Detail:**

When this quick action is selected then the Withholding Tax Batch Detail dialog will be opened. From here we can select the withholding tax batch whose detail we want to see and it is displayed in the grid.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc7l622vc6y-soU0HcLRhWarGG8Cl5Y0rTWdoZuKuWCYf_A6nW4dzm53Wp8P6KNE3GdyeHuppd7qSNs2AtQVLrVknVTEYzah8PSvX5VeaenUj5PY2iW3RGvIKbp2CK4LwJ6l_1YrCkPdswC_s8e2ZUMINk?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

**Create Withholding Tax Batch:**

To create a new withholding tax batch click on ‘+’ and a new dialog is displayed. Enter the date range for which we want to make the IRS payment. Now select the RTOs for which we want to make the IRS payment and click on ‘Create Withholding Batch’ to create the withholding tax batch.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXexPAQ-FuHogsqPzMD4dQ9oQFQwGfQklfsIp6PgbokO0d-VMzGpHcXZV50TdPy3QHwbvGo2rKVjMZF5sqanA9tCFO0I4JCCPb7ZcOVzZiMgmfE5iGNXEWdrs6MxbvEr7TVEv2c3sjfVBdkkTU8s73PCvQ_Z?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>



**Account Register Changes:**For each RTO, two account registers are created:

* First, the withholding tax is moved to the account register, creating an account register of type ‘Withholding Tax’.
* After this, an IRS payment is made, and another account register is created with the type ‘Withholding Tax Payment’.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcxXM9cYb7lTUyvTBhwk8TNw6QA6wZWAVPa-F21inJPGbGys9Kqg9IvEldYc9mnkGk6RugCDpjpGprZrks0v4Hgd_b9gDqBkqSiIpLey2bg4iycY6HS1rmM_sSzPr5S3jygrFu2j5SzQ7hvPTR8m4CHOLs?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

### **Reverse IRS Payment:**

The Payment made to the IRS can be reversed from RTO detail ‘REVERSE IRS PAYMENTS’.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcvI7Bi0bW3iitMJqgIaNRm8cH-C5hSIGenbaZ9Fm6JfcRYZkN-xFh_db1ngzdAi7TqkRelCBAHR4wr-4aVjTADsnTerdCAy8jzClwVBmKkRYd5tiMVPIl0GAUi159SbxUDqYb8Jgm5CJz8GxTi353dVbFV?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

**Account Register Changes:**

When an IRS payment is reversed, three account register records are created:

* A reversal record for the account register ‘Withholding Tax Payment’.
* A reversal record for the account register ‘Withholding Tax’.
* An account register with the type ‘Withholding Tax Refund’ is created (which can be used for ‘Account Transfer’ or ‘Withholding Tax Refund’).

If withholding tax from selected entries was used to pay a single ‘Withholding Tax Payment,’ then a single set of reversal account register records will be created. Otherwise, the number of reversal account register records created depends on the number of ‘Withholding Tax Payments’ made from the selected entries.![](https://lh7-rt.googleusercontent.com/docsz/AD\_4nXeG\_XNqWIVY69bbHRsThszoch437i43dPcU2wN6HAk2XPKHCXHXRtgka2wfqWi0fzY\_YJ9us004sm88qtYV59r5O4Kxvs3UeOZ0WTc\_wAggwtKM8ilNIqtYtJGVeWQ6fGziM5GVyKLdkUv\_9moT6UPW-Ffj?key=rVub6YkZBoq-An-SBd1GRg)

### **Withholding Tax Rollback When Prize Money is Rolledback:**&#x20;

When the trip is rolled back then all the account registers with type ‘Withholding Tax Refund’ associated with that trip’s withholding tax is rolled back.

**Account Register Changes:**

* Reversal account register created for each account register (Withholding Tax Refund).
* Reversal account register created for all ‘Account Transfer’ done from ‘Withholding Tax Refund’ account register.



Let consider the trip highlighted below its withholding tax was used for ‘Withholding Tax Check’, IRS payment (Withholding Tax Payment) and entry payment (Account Transfer) and the this is rolled back.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfexwRDDiPEVkIAO2in3o3oNF4QnQp3TgiE78aYdIFxIdExFrHtKCzGLTxx8nsvE0VbmZlkE5kbiLcRYCoPKDtjz8pATepC-RM2Dz40vG8a180vCoaaxchQ6MwnEofwPBqMDZgNBQ_4MALZg_NvwtPfNqo?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

When the trip is rolled back then&#x20;

* The ‘Withholding Tax Refund’ account register highlighted in above screenshot will be reversed and reversal account register record will be created with type ‘Withholding Tax Rollback’.
* The entry payment made from this ‘Withholding Tax Refund’ will also be reversed and reversal account register record will be created.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcog21t2vCFAvYGo4dzWqeDuPrmh4PH1yrfsChfCUuGpeD4AddyTyWLoaz43DM-uyhxoCKVsH0eWIkzdoOS2tjhhli6w3Nrb7Ga_oktmCuEIAQsZkUpdOh3XlYQw37uqqOBrb16k77_8ciUd1P5OOPsc6E?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>
