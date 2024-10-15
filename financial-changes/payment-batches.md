---
icon: money-bill-wave
---

# Payment Batches

* Step 1: Move Credit From Account
* Step 2: Checkout Entries
* Step 3: Create Payment Batch
* Step 4: Post Payments

#### **Step 1: Move Credit To Account**

In 'Move Credit to Account', we can apply unapplied prize money and transfer the credit balance of the entries to the Account Register as ‘Balance Refund’.

&#x20;**Entries Grid:**

* **Columns:**&#x20;
  * **Type:** This column indicates the type of credit moved to the account register. If the entry has only prize money or balance refund, the type will be ‘Prize Money’ or ‘Balance Refund’ respectively. If the entry has both prize money and balance refund, the type will be ‘Both’.
  * **To Be Paid:** This will be the sum of the prize money and credit balance (balance refund) moved to the account register for the entry.
* **Color Coding for Rows: Entries are displayed as red in the grid because:**
  * The amount to be paid is zero, or
  * ‘Require SSN for Prize Money Pref’ is on and PMR is non-foreigner and has no ssn and federal id.

**Move Credit To Account:** We will select the entries for which we want to apply the prize money, transfer the balance refund, or both. Then we will click on ‘Move Credit to Account’. For the selected entries, we will perform the following operations:

* **Apply Prize Money:** If selected entry has unapplied prize money then we will apply prize money for that entry. The details for ‘apply prize money’ are mentioned in the Apply Prize Money section.
* **Transfer Credit Balance:** If selected entry has credit balance then, we will move that credit balance as ‘Balance Refund’ to A/R for that entry. The details related to ‘Move Credit To Account’ are mentioned in its related section.
* **Move to Payment Batch Step 2 - Checkout Entries:** After the prize money is applied and the credit balance is moved to A/R as ‘Balance Refund’, we will be automatically switched to _‘Checkout Entries Tab’_.

**Credit Summary:** This summary shows how much credit (prize money, balance refund) will be transferred to the account register for all the selected entries.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfUbZ6aEQxnx7M2h9L8PSOW-KsnC6aXnyd8Wzb9h5qUD5ChLnTN-oUIyzneFrDXyMm497XDQj5wFHeteiId4wsu9B2SSFgH1VafWwJhbIz-NZpag155pTPSZ41n86XJlj8t6qlFJqVVKexdLcsQix7aKAjZ?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

#### **Step 2: Checkout Entries**

**In ‘Checkout Entries’ the entries having a debit balance can be paid using the account register credit.**

**RTO Grid:**

* This grid shows all the RTOs whose related entries (where the RTO is set as PMR/RP) have a debit balance for the selected show.
* **Color Coding**: RTO data is displayed in red if,
  * There is no available credit (reasons are listed in ‘Checkout Entries with Account Register Credit’), or
  * All the related entries for the selected RTO have a PMR/RP mismatch error, meaning they cannot be paid by the RTO.

**Entries Grid:**

* When an RTO is selected, all entries that have a debit balance and where the selected RTO is set as PMR or RP will be displayed in the right-side grid.
* Whenever an entry is selected then the column ‘Applied Amount’ is updated for that entry based on available credit.
  * If the entry’s balance is less than available credit then ‘Applied Amount’ will be equal to the entry’s balance.
  * If entry’s balance is more than available credit then ‘Applied Amount’ will be equal to the available credit.
* If an entry is selected and there is no available credit left to pay off other entries, then their checkboxes will be disabled.
* **Color Coding**: Entries are displayed in red if,
  * There is an RP/PMR mismatch error, or
  * The RTO associated with the entry has no available credit.

**Summary Section:** This section shows the available credit for the selected RTO and the total account register credit that will be moved to the selected entries from the selected RTO’s account.

**Checkout Entries:**&#x20;

When some entries are selected and 'Checkout Entries' is clicked, the credit will be transferred to the selected entries from RTO’s account register.&#x20;

Checkout Entries tab will be updated to remove the RTO if all of its entries are paid.



<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe8Xvmogrb3C1_uhgK6dwUeTU2JbhID3gKY8wqVDV-1WCRzcuLi8LzNPMJe0mC3r6FSd1PRHZ7QCX9DPDXbIWV11520ekwhM5sWVSsKeeMEDIfyjBrtEEtURFgWBEx44wjYWFCHjEI9H1Cyfks0qIJNaAA?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

#### **Step 3: Create Payment Batch**

In this step we calculate the payable credit for RTO’s, display the RTO’s show credits and payments information and create payment batch for selected RTO’s.

**Batch Type Button:** There are three buttons present in ‘Create Batch’ to create three different types of payment batches.

* **Prize Money Only:** When this radio button is selected then only those RTO’s are displayed in the grid that have earned some prize money in this show that can be paid as _‘Prize Money Check’_.
* **Balance Refund Only:** When this radio button is selected then RTO’s that have ‘Balance Refund’ that can be paid as _‘Balance Refund Check’_ will be displayed in the grid.
* **Both:** In this case, RTO’s that have non-paid/ non-used ‘Prize Money’ or ‘Balance Refund’ will appear in the grid. The generated check will have the type _'Prize Money Check'_ if at least one prize money is included in this payment batch. If we are only paying the balance refund, the check type will be _'Balance Refund.'_
* _**All:** If the ‘All’ radio button is selected, all the RTOs for which some credit was moved to the account register for the selected show will be displayed in the grid._

**Columns:** &#x20;

* **Prize Money Credit:** Total ‘Prize Money’ earned by the RTO in the selected show. This column is displayed for batch type _‘Prize Money’_ and _‘Both’._
* **Balance Refund Credit:** Total ‘Balance Refund’ transferred to RTO for selected show. This column is displayed for batch type _‘Balance Refund’_ and _‘Both’_.
* **Total Credit:** This will be the sum of ‘Prize Money Credit’  and ‘Balance Refund Credit’. It will only be displayed for batch type _‘Both’._
* **Payable Credit:** Following list of calculations are performed to calculate the payable credit.
  * **Calculate Total Credit Amount:** Sum up the amounts from credit account registers (where the amount is negative). The type of account register depends on the selected batch type.
  * **Exclude Non-Transferable Amount:** Subtract the total amount for non-transferable  account registers from total calculated in step 1. If RTO do not have valid taxform membership then all credit account registers become non-transferable. If RTO is non foreign, ssn and federal id then all ‘Prize Money’ account registers become non-transferable.
  * **Exclude Check and Entry Payments:** Subtract the check and entry payments from total calculated in step 1. The remaining total after exclusions is the payable credit.
  * **Adjust Payable Credit for Account Balance:** If the balance after payments is positive, and the Payment Batch Preference is set to 'Credit Balance Only' then,
    * Calculate the available balance by adding the total account register balance till selected show and the total debit entry balances for current and past shows where RTO was set as RP.
    * If the available balance in the account is less than the previously calculated payable credit, then set the payable credit to be the available balance.
  * **Validate Credit Payable:** Credit Payable will be set to zero if,
    * Credit payable is greater than zero.
    * RTO has non verified ‘Taxform Membership’.
* **Balance After Payment:** This is calculated by subtracting the 'Payable Credit' from the 'Account Balance' (total of account registers and entry balances for current and past shows where RTO is set as RP). If the resulting balance is greater than zero and Payment Batch pref is set to ‘Credit Balance Only’, we then recalculate it by subtracting the 'Payable Credit' from the 'Account Balance' (total of account registers and entry balances for all shows where RTO is set as RP).
* **Status: An RTO can have one or a combination of the following statuses**
  * **Taxform Status:** The 'Taxform Membership' status is set as the RTO status. We can override this status with the statuses below if 'Taxform Membership' is verified.
  * **SSN/FID Missing:** If the RTO is taxform verified, has zero payable credit, won prize money (transferred to A/R), is non-foreign, and has a missing SSN or federal ID, the status will be set to 'SSN/FID Missing.'
  * **Balance After Payment:** If the RTO is taxform verified, has some payable credit, and the balance after payment is greater than zero, the status will be set to 'Balance After Payment.'
  * **On Credit Hold**: If the RTO is on credit hold then this status is shown.
  * **Pending Account Register Balance:** This status is shown when RTO has debit account register balance.
  * **Fully Paid:** If all the credit moved to the account register is used for entry payments or rto payment then its status appears as fully paid.

**RTO Summary:** Whenever an RTO is selected in the grid, the credits earned in the selected show and their usage are displayed in the RTO Summary section. By default, the RTO Summary Grid displays entries for past and current shows. The RTO Summary Grid is updated when we click on some RTO Summary label to display related data (for example: if we click on ‘Account Register Balance’ then all the account registers for selected RTO will be displayed in RTO Summary Grid ).

* **Credits:**
  * **Prize Money Credit:** Total prize money earned by the RTO in the selected show.&#x20;
  * **Balance Refund Credit:** Total balance refund earned by RTO in selected show.&#x20;
  * **Total Credits:** Sum of prize money credit and balance refund credit.&#x20;
* **Adjustments:**
  * **Not-Transferable Portion:** Sum of non-transferable account registers.
  * **Total Payments:** Sum of check and entry payments made in selected show.
    * **Check Payments:** Total check payments made in selected show.
    * **Entry Payments:** Total entry payments made in selected show.
  * **Remaining Credits:** To calculate the remaining credit, subtract the entry and RTO payments from the show’s available credit. If the result is less than zero (i.e., payments made are greater than the available credit), the remaining credit is displayed as zero.
* **Other Factors:**
  * **Account Register Balance: Sum of account registers for all shows.**
  * **Entries Balance: Sum of entries sum for current and past shows where RTO is set as RP.**



**Color Coding For Rows:**

* **No Color:** RTO has ‘Payable Credit’.
* **Red Color:** RTO has no ‘Payable Credit’.
* **Yellow Color:** RTO has ‘Payable Credit’ and credit ‘Balance After Payment’.

**Create Payment Batch:**

* Select some RTOs to which we want to make the payment and click ‘Create Payment Batch’.
* A new account register record will be created for each selected RTO to show the payment made.
* After the payment batch is created we will automatically switch to the Post Payments tab.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcFgumG1Z85hvaUhakczgvT5WQvEacQBMeUVxbkkGB8APL5WLBYqSm9_v6A4ewh84EgzY-ta1oti_03O9eE6c24nMFEajYLxmxJX1OI1p2KwF3YsFKe8j8fVgE7ZeT30BqPR5US4ZizNbTI85pAWnaFX6s?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

#### **Step 4: Post Payments**

**Unposted Checks Tab:** **Fields Updated:** In this tab, you can update the check number, type, and description for batch items.

**Post To Account:** The selected batch items are posted when we click on ‘Post To Account’.&#x20;

**Example Description:** When a check created in 4D is posted then a new account register record will be created. But for checks created in cloud no account register record will be created (as it is already created in ‘Create Batch’ step).

**Reversed Amount Dialog:** If we have a non-posted check (created in cloud) that includes prize money/ balance refund, and these amounts are reversed due to PMR/RP or other reasons, a dialog will appear when posting the check, displaying all the reversed amounts.

Note: after the unposted checks are posted we are automatically switched to ‘Posted Checks Tab’

**Delete:** The selected batch items are deleted when we click on ‘Delete’.



**Example Description:** When a check created in 4D is deleted then there is no change in the account register. When a check created in the cloud is deleted then a new account register is created.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXePd3zh-51f4KTZ4Q1tsuFus2Uo-Jknz0_NSbi5EnvLWBenrLm3jl5ZsjOlbYPlQBCUQcaEfW3_D9rPuSHIozq2x7eF7nUQPLTiOWpSEyEh4U5Mazarlg5L9-62dsxaR2YWTlOtD00MRTgHhmCmFDgUjo8T?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

**Posted Checks Tab:**

**Fields Updated:** Check number can be updated in this step.

**Void Check:** In the new financial system instead of updating the amount for account register related to check to zero. We create a new account register records for voided checks.

**Color Coding:** Voided checks are displayed in red.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcAVj6yc4f96ewsqS59Vn3UQe787i_H8_SzyLObW0ABawLmELJdlLL9nS6Hc60_FjrzfxD6OCPgryU-3bvs5cS9zv3p83yjP_Z6tFTfSpygY6Vx5fJlCmOfe-DXonIO1xQun91G63tEGT8-Jy3MqoZYhiRK?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

**Batch Summary:**

* **Unposted Checks:** Sum of the unposted checks amount.
* **Posted Checks:** Sum of the posted checks amount.
* **Total Checks:** The difference between the amount of voided checks and the sum of unposted and posted checks.

**Voided Checks:** Sum of the void checks amount.
