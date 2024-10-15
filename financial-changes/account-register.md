---
icon: abacus
---

# Account Register

## Account Register Detail Dialog

Whenever we double click on the account register detail dialog is displayed. The grid shows the sources and destination for the selected account register record.

**For Account Register Creadter In 4D:** The account registers created in 4D have no source and destination so nothing will be displayed in the grid.

**For Account Register Created In Cloud:**&#x20;

* **Credit Account Registers:** The account register created when credit is transferred to the account, such as for prize money, balance refunds, withholding tax refunds, etc.
  * **No Credit Used:** When no amount is transferred from the selected account register to any entry or RTO, no destinations are displayed in the grid.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcGsp3yvptoQyVn8-u37T-fwwrhw4kYfKxA40_4M1WwIiVeDFcFiThSisEQSMKAPJ6mPZmnXmgFFLuSAPaaJBFPzstiDLO_rsszD8LIhOTOb2WdHt3A6qtWIOb26V9ZwtuYr1tPWDgM8517ma5hgQLyGcuv?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

* **Credit Used:** A list of destinations is displayed when you double-click on an account register that was used to pay off multiple entries or create a check.
* **Reversed:** If the current account register is reversed due to prize money rollback, payment reversal, or PMR/RP change, then along with destinations, the reversal records for the current account register and destinations are also displayed in the grid.
* **Debit Account Registers:** The account register created when credit is transferred from the account to an entry or check, such as for account transfers, prize money checks, balance refund checks, etc.
  * **Non-Reversed:** The sources that were used to pay the current account register are displayed.
* **Reversed:** If the selected account register is reversed, the reversal record is also displayed in the grid along with the sources.
* **Reversal Account Registers:** The original account register that was reversed to create the current account register is displayed in the grid.
