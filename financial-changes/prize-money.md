---
icon: award
---

# Prize Money

## Introduction

There are a nuumber of changes to how prize money is managed in the system.  These changes are designed to create better compliance with tax status of prize money recipients and to reduce the number of cases where prize money gets reversed and reapplied.

There are some very important new features that make managing prize money easier and more accurate.

## Flow of Prize Money

In the old system prize money flowed in a particular way in terms of transactions.  The following diagram shows how money from prize money would applied to an entry.  Any remaining credit would then be transferred to the account register and ultimately result in a prize money check.

<figure><img src="../.gitbook/assets/prixemoney-old.jpg" alt=""><figcaption><p>Old flow of prize money</p></figcaption></figure>

In the new system the way prize money flows is different.  For starters we have elected to leave prize money unapplied and stored in the class until generally later i the process. The goal of this change is to only utilize prize money at the time its needed to be paid.  By doing this we hope to reduce the number of transactions that occur to reverse incorrect prize money and generally have a more streamlined and simplified transaction history.

When prize money is utilized it first is applied to the account register of the prize money recipient.  Once it is applied there we then determine if the necessary tax information is in place to make the prize money payable.  If it is payable then it can be transferred as a credit to pay an entry balance or to be issued as a prize money check.\


<figure><img src="../.gitbook/assets/prizemoney-new.jpg" alt=""><figcaption></figcaption></figure>

In this example prize money is applied to the account register of the prize money recipient.  A portion is then transferred to an entry as a payment and the remainder is paid in a prize money check.

## Rolling-back Prize Money

In our old system when prize money was applied from a class all entries would have prize money applied.  If there were changes in results or prize money all placing and prize money had to be reversed and the reapplied.

In the new system it is now possible to rollback prize money for individual placings.

<figure><img src="../.gitbook/assets/Class-prizemoney-rollback.jpg" alt=""><figcaption></figcaption></figure>

## Entry - Prize Money Summary

We now track a prize money summary on each entry to make it clear the status of prize money.

Whenever prize money is applied or rolled back, the prize money box is updated in the entry detail.\


<div align="left">

<figure><img src="../.gitbook/assets/prizemoney-summary.jpg" alt=""><figcaption></figcaption></figure>

</div>

### Definitions

* **Won:** The total amount of prize money won by the entry.
* **Unapplied**: Prize money won by the entry but not yet applied.
* **Applied:** Prize money won by the entry and already applied
* **Tax Withheld:** The withholding tax deducted from the prize money won when it is applied to the entry.
* **Payment Applied:** The amount of prize money used to pay off the current entry.

***

## Transfer Prize Money

**Areas:** Prize Money can be transferred to account register from following areas.

* Class Detail
* Entry Detail
* Transfer Prize Money to PMR Quick Action
* Payment Batch - Move Credit To Account
* Add Payment From Entry
* Apply Payments Quick Action

**Note:** Prize money can be transferred to account register from all the above areas, but the prize money payment is applied to the entry only from ‘Add Payment From Entry’ and ‘Apply Payments Quick Action.’

### **1 - Class Detail:**&#x20;

Prize money can be transferred to account register by clicking on the ’Transfer'

<div align="left">

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

</div>

When prize money is transferred, the class is saved first, and then the prize money is transferred. Once the prize money is transferred, the trip will be locked, and the trip data cannot be updated.

<div align="left">

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

</div>

Note: Trips with unapplied prize money can be updated.

### 2 - Entry Detail:&#x20;

Prize money can be applied from ‘Prize Money Action’ present in Classes Tab.

<div align="left">

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

</div>

Once the prize money is applied then _‘Prize Money Action’_ will become unselectable and a message will be displayed.

<div data-full-width="true">

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

</div>

&#x20;The Prize Money Box will be updated to show the prize money applied.

<figure><img src="../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

**Note**: Prize money changes will be saved when the entry is saved.

### **3- Quick Action**

Prize money can be applied from Entry’s quick action _‘Transfer Prize Money to PMR’_.

<figure><img src="../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

### **4- Payment Batch - Move Credit To Account:**

In ‘Payment Batch Step 1 - Move Credit To Account,’ all the entries where prize money is not applied will be displayed. Select the entries to which you want to transfer the prize money to account register and click on ‘Move Credit To Account.’ Prize money will then be transferred for those entries. This process is explained in detail in the respective section.

<figure><img src="../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

### **5- Add Payment From Entry**

In the ‘Add Payment’ dialog, there are two checkboxes

#### **Transfer Prize Money to PMR**:

* The amount displayed next to this checkbox represents the total unapplied prize money for the current entry.
* When this checkbox is selected and the 'OK' button is clicked, the prize money is transferred from class to the account register (PMR).

#### **Apply Prize Money Payment from PMR**:

* The amount displayed next to this checkbox represents the unused prize money currently available in the account register (PMR). If the 'Transfer Prize Money to PMR' checkbox is also selected, then the amount displayed here will include the prize money that will be transferred to the account register.
* When this checkbox is selected and the 'OK' button is clicked, the amount displayed next to this checkbox is applied as a payment to the current entry.

**Note:** This process is cumulative: if both checkboxes are selected, the prize money is first transferred to the account register and then applied to the entry as a payment.

<figure><img src="../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

### **6 - Apply Payments Quick Action**

This action is similar to the 'Add Payment' functionality, with two checkboxes available to manage prize money.

* Transfer Prize Money
* Apply Prize Money Payment

**Color Coding**: If the ‘Available Prize Money’ is displayed in red, it indicates a restriction or condition—such as missing SSN or Federal ID—that prevents it from being applied as a payment to the entry. However, we can still transfer this amount to the account register (PMR).

<figure><img src="../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>



### **Account Register Changes**

Whenever prize money is applied following account register changes takes place

* **Add Payment/ Apply Payment:**&#x20;
  * **Transfer Prize Money Checkbox is Checked**:&#x20;
    * When this checkbox is checked, a new Account Register record is created for each trip where prize money is transferred to the account register (PMR). This means that if prize money from multiple trips is being transferred, separate Account Register records will be created for each trip.
  * **Apply Prize Money Payment Checkbox is Checked**:
    * If the current entry has a debit balance, an Account Register record is created when the entry is paid off using the prize money.&#x20;
  * **Both Checkboxes are Checked**: When both checkboxes are checked:
    * **First**, a new Account Register record is created for each trip whose prize money is transferred to the account register.
    * **Second**, another Account Register record is created to show the prize money payment made to the entry.
* **Other Areas:**&#x20;
  * For all other areas (class/ entry detail, quick action, payment batch) a new account register record is created for each trip to move the prize money to the account register but no prize money is used to pay off the entry.

***

## Checkout Entries with Account Register Credit

### **Prize Money Payment:**

Each entry can be paid using its unapplied prize money or unused prize money present in the account register from

* Add Payment From Entry
* Apply Payment Quick Action
* **Account Transfer: Entry can be paid using account register credit from**
  * Move Credit From Account - Add Payment
  * Payment Batch - Checkout Entries

### **Prize Money Preferences**

Following preferences are used when applying prize money payments

* Apply Prize Money Payment Despite RP/PMR Mismatch
* Require SSN for Prize Money
* Auto Apply Prize Money

### Accessing Preferences

Users in the administrative group have access to these settings.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfpsDu4qj74vYShLVq9LgS5s0_ptZlDQBPby8exkCVfeW-EBNjhgi1wRbp90se12_Z6Bga-NpCvtNk9Zungg-3bGxNzgwMEQ_A_MH4PljVOVOeYr15aka9_mTW0ETlpYnCVMcVhWYSTPUEgQPLWy6xDCtBt?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

#### **Apply Prize Money Payment Despite RP/PMR Mismatch:**&#x20;

* If the preference is off and the entry has different PMR and RP, ‘PMR’ credit cannot be used to pay off the entry.
* If the preference is on, then ‘PMR’ credit can be used to pay off the entry despite the PMR/RP mismatch.

#### **Require SSN for Prize Money:**

* If the preference is on and the PMR is not a foreigner and does not have an SSN or Federal ID, then no prize money credit from the RTO’s account register can be used for entry payment. The entry can only be paid using a balance refund.
* If the preference is off, then we can use all the RTO’s credit to pay off the entry despite the SSN/ Federal id missing.

#### **Auto Apply Prize Money Pref:**

* If the pref is ‘off’, then the Apply Prize Money checkbox will not be automatically checked when the dialog is opened for add payment or apply payment.
* If the pref is ‘on’, then the Apply Prize Money checkbox will be automatically checked

### Paying an Entry with Prize Money

**Add Payment:** Entry balance is greater than zero and all other conditions to apply prize money payment (as discussed below) are met.

<figure><img src="../.gitbook/assets/PrizeMoneyPayment (1).png" alt=""><figcaption></figcaption></figure>

\


**Validations:** The following validations should be checked before moving the credit from the account register to the entry.

* **Valid Tax Form Membership:** If taxform lookup is enabled for the company and the tax form membership is not valid, RTO’s credit cannot be used to pay off the entry.
* **Pending Account Register Balance:** If the RTO has a pending account register balance, no account register credit can be transferred to the entry.
* **On Credit Hold:** No account register credit can be transferred to the entry if the RTO is on credit hold.
* **SSN/Federal ID Missing:** If the ‘Apply Prize Money Payment Despite RP/PMR Mismatch’ preference is off, and the PMR is not a foreigner and has no SSN or Federal ID, then prize money in the account register cannot be used for entry payments.
* **RP/PMR Mismatch:** If the preference is off and the entry has different PMR and RP, PMR credit cannot be used for entry payments. Consequently, no prize money payment can be made to the entry, and the PMR checkbox will be disabled in ‘Move Credit From Account.’

**Apply Payment:** No additional conditions required. Checkbox will be checked automatically.

**Account Register Changes:**

* **4D or Cloud Credit:** When an entry is paid using either 4D credit or Cloud credit, a single account register record will be created.
* **Combination of 4D and Cloud Credit:** When an entry is paid partially with 4D credit and partially with Cloud credit, two separate account register records will be created.



### Prize Money Examples

**Example 1 - Entry has debit balance (Add Payment From Entry)**

Entry 19740 has one unapplied prize money. The following actions will be performed when we apply this prize money to the entry:

* $110 will be moved to the PMR’s account register.
* Then, the $110 will be transferred from the account register to the entry to pay off the balance. The entry’s balance will be reduced from $1025 to $915, as shown in the screenshot below.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdIa6ziWbnlIChFpRf_Ikf-8jBt4fUnhE-kM3rYDtGD2RkyCzaxCl-lbeI0r_DCUELVNhEUcLZ4_RYZP-nyN6jeU_0DkDknuaKXxg03l9K8fMKtoyjHbxW7XLdm9GHTE1e4JOyDbbk3julvcQHard2J7aw?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

#### **Example 2: RP/ PMR Mismatch (Add Payment - Move Credit From Account)**

Entry 19740 has a debit balance, but we can’t move credit from the PMR account register because the PMR is not the same as the RP. That’s why the PMR’s radio button is disabled.

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

#### **Example 3: Credit On Hold (Apply Payment)**

Entry 3610 has a debit balance, but we cannot apply prize money payment to it because the RTO is on credit hold.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdWJkj5UUeL1y2EUtczn6qzIXTdVIDRVaykIEBjpXOypxbbHMjdSP-mom385m-rLQu0B_ErzB7-I15LdpRbblZ8B1sSxfGX2QIyNLpkVMO11ts699-vwTn2y6CEVdMf_Wcnb3NwIsq4kfLO5pbexuma4RGw?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

The prize money can be applied for this entry but the applied prize money cannot be used to pay off the entry so ‘Available Prize Money’ is displayed in red and ‘Prize Money Payment’ is 0.

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe9Hs6oxjHJmr0EwufERw-nOMxdkWAWtiJsOCxGpuhlUYZO3gjHXyOit7IHQy6TftpZWCFDbEX_vLWuD2N3Uc8TS7nWAh1QipcAqDGI0yGe0NovnYUzs-1kzhiA-MqgdVSxnyVItNfHbA90ZTdp-WSPdkUB?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>



***

## Rollback Prize Money

**Areas:** Prize Money can be rolled back from following areas.

1. Class Detail
2. Entry Detail
3. Rollback Prize Money Quick Action

{% hint style="info" %}
Importa
{% endhint %}

**Prize Money Applied in 4D and Rolled Back in Cloud**

&#x20;If prize money is applied in 4D and then reversed in the cloud, the following actions will take place:&#x20;

* Reverse the prize money payment made to the current entry.&#x20;
* Reverse the prize money moved to the Account Register.



#### **Example 1: Prize Money Applied and Current Entry Paid with This Amount**&#x20;

Consider entry 1523, where two prize amounts were applied, and they were used to pay off the current entry.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdQYwygoKzUG-1U3jNVzcjsOONxdt3TLtABQ6U_LI73Ghcwinira6-ni8UgxQAyD4NGopebqeLb0EJV9EvWBUIPFaOZaO5QcMyUqwsPcqUgcwuz69rGctnEDpo55T4j8y_UCIh4crRutrm8kGYFHh1WbIho?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

When these prize money is rolled back, then

* All the prize money payments made to this entry will be reversed.&#x20;
* The prize money box will be updated.
* The entry’s balance will be updated from $10 to $885.

**Note:** Since no prize money was moved to the Account Register, there will be no change in the PMR’s Account Register.

#### **Example 2: Prize Money Applied and Amount Moved to Account Register**

In entry 5083, $1390 of prize money was applied to the entry, and all of it was moved to the Account Register. The screenshot below shows the payment records created when prize money is applied in the entry and the Account Register record created when the prize money was moved to the Account Register.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeXvsi7KpHapZvvCuBmTyZ1bsgW-l8OOdFl6QQqid3WSAGFcNvMiAlDV_84XnauEHeF8kNH1crFwrgGzH5O1QjuXiKF66NQy1MfXbmxcH2LKpCNoH220wzu9ScJX9d75NTsEtpim_G84seLgf7iXJYWx0nz?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcUt7P3pU090xTY8eFbm8za6tjCT7nr80nAEeXhWwVUVqxnihDHGKdLyO6ezngREfKLJSnoWa-8CnweKC8b7JF-oJZoks7UHvRjgHtbEPaF5rCdmT2QlYOUThVOTZituo_9FQ2mDkDH68z-Mi11sael6Dk?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

When this prize money is rolled back,&#x20;

* All the amount moved to the Account Register will be transferred back to the entry. Creating a new Account Register Record.
* The prize money payment made to the entry will also be reversed by creating new payment records.



<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeS68lJn0LoLtCSDmyeScvSYw8x6-nTuz5vPQr2kIJeBl2zwBZ79BGh7SaWanMqhlCBvTljcVt8JFFk-N03_XGLEbgPxnWsJn1zR2gl2UpsXHSixoqQYiEuMUuwAYpJBttyz1FrMRTy3k7D-h2E-HlFrQMq?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

**Note:** There will be no effect on the entry’s balance, but the Account Register balance will be updated from -$1390 to $0.

**Prize Money Applied in Cloud and Rolled Back in Cloud** If prize money applied in the cloud is rolled back, the following actions will be performed:

* Rollback all 'Account Transfers' made from that prize money amount.
* Rollback all 'Prize Money' from the Account Register for trips that are rolled back.



**Example 1: Prize Money Applied, No Payoff Performed**

In entry 981, $100 of prize money was applied, but no payoff was performed from this amount. Therefore, this amount is currently present in the Account Register.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfvUKsSDOsjPhck8OL30iMFefGf80LogBoJIWgi2akOjaYudZ32Gshhm9uOwZ8da80wiFfdGHlHZU9OwFMqrhto78l9VtUkdsaXs2EIiKfrJd_ZkRBoDqpSIaEURTSov3glexxE9awugKg83YwVJ1MZWGoJ?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfpDsPbu1pzZ6-CUX5ymy8l5dn2GB8b5LHBzt-y0iUQuFTCIu1-SgZf-Yhy58nuZnw3Ue42-_AEO5P085kIjXk3yInC6z5o8Hnbe3Naap95Nrbxq10W8N6HHulwW5QoUCAZJ7DnLijhbaPjvoyERe9idYc?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

When this prize money is rolled back,&#x20;

* We will simply rollback the prize money that was moved to the Account Register, creating a new Account Register record for PMR and updating the account balance from -$100 to $0.&#x20;
* The prize money box will also be updated to reflect the rolled-back prize money.

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>



**Example 2: Prize Money applied and multiple entries paid with this amount**

Consider entry '1162', where a total of $75 in prize money was applied. Out of this amount, $10 was used to pay off the current entry, and $50 was used to pay off another entry '1163' using 'Move Credit from Account'. The screenshot below displays the entry in which prize money was applied and the PMR’s Account Register records created when entries were paid off.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdWIbOyAzgW5fn4zoC0mE15BxeHHes5d6AXIx10Xl80fJpPAipb_f_Vn81Liw5zMmccZcaO2XePxPrC5yTToX3OVb_feXP-tUG89YNHrin1gUFelIP1vnx3QDCcQSfrpCF-ADAg4wDosQjne1j4g9HN0i8v?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXenkfjFLmkC3aRqV-GgoXCAb7xL-AzpOQpFomBRd_rzwpAGViakqJafjQ1yeTTs4rDGRjRvZFNI6zx7fRla91RrOJu4z2rH-l77cpM_NVcQgUZeM1MyeAQK_VoiYP_iBT-jCs1s42uyvWDb65kAJnbnce4?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

When the prize money applied to entry '1162' is rolled back,&#x20;

* The prize money payments/ account transfers made to entries '1162' and '1163' will also be rolled back, as they were made using entry 1162's prize money.

Entry ‘1163’ balance will be updated from $0 to $50 as prize money payment of $50 is reversed from it.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXel5kN0teIi6bM2CguS_CMlZjxtGd4jiU20ofCRi4Mtd6sI4q7nmLGE5qipnt5OJl7nILzUloDF-RCLRCgRGHxnf3WaArHVf-8DcKYzXORLIb50xMIVs3pvZ4bwImbg43gHqb5TxIbRhVCJTHiu-TQaZgAS?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

For Entry ‘1162’ balance will be updated $0 to $10 as prize money payment of $10 is reversed from it.

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

* Following _Account Register_ records will be created for entry ‘1162’ prize money rollback.

<figure><img src="../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

**Example 3: Prize Money Applied and Check Was Paid**

In entry '1799', $20 prize money was applied and then this prize money was paid to RTO as a Prize Money Check.

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeA5R4lLTBiN9n9h6SDK9ZkkkWo0Wsxii1-lz9ld1ETPN6iDvBjwPW6lMhs45GblSV6lbqktTFDVGvkrwXIokliHYSAjcBhEhGCreFVBDcKcxA2SztzTjCy3dy22kMYCoSKwMhPePyu8jxXDpeb-UEWsZkK?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

After this the prize money was rolled back. We will rollback the prize money moved to the account register but the payment made to the RTO as Check will not be reversed. Following Account Register will be created.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeGd_1yv7TRsEmm2Mx8ciq1iAt9cu5ud1k6pRGyDojqmDh0Om4-CWrnfTiabrMAFWCCWU1Toz4eERGDqdAfJRVu3CXCRFucXm9MtZEQC_22hncrpmmRfl6qbL5QyGMv1zJRlGJywWVp9K_51yZf7YSAklqg?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

**Note:** As the $20 transferred and paid as a Check are not reversed, they will remain as an anomaly in the system, resulting in a debit of $20 in the Account Balance.



## Reverse Account Register When Payment is Reversed

If a payment has a related account register record and it is reversed, then the related account register record will also be reversed.

**Note:** Payments of type ‘Prize Money’ cannot be reversed from the payment detail.



**Example : Reverse a payment that was paid from using multiple account registers**

In entry 51, $100 is applied as ‘Account Transfer’.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfUMHoFjuLcn1f1QvxLmeibO45HatsWAr_NUCL8XoThPETxu5VP3TGVm0C206M3CaX-3aX-NmzEPs0LIAuK8Wpl8fQnMBh6-NV8oEvrwJTtPv2GApanzEzwcEiD-BWcLRCqEm6RJaJll3LSrjeK2l0xUPE?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

This $100 was paid using two different ‘Balance Refund’ account registers. These account registers are highlighted below

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXetcnjXtBV59UnebNeheDD8WQ_GktT9BmZR2Q3K9ZwRUBWHFNOkcuG38l3l-RbN79Nvb-dD4sKXI5zQhIDBX-QuMNOOkdP162XazPsgGqxjXkgC8FK0R2n59LFmrE2hM0Uwfiy-r1MdvhwaxlBBbJxd3-VL?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

When we will reverse this ‘Account Transfer’ from payment detail&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdM8EsSWJwa0vfH-4sdr_ZzJelOCLi5vVOxZlFNrupV5nFsLevVfuSYEOmVxBmpzbPRkALBSmBdhXulDdlss_BEIDrv5YyB5V2e5hH5RqBYXNnastVhnR8URZH8Y6Ev1rrg2KRNYkNYcVkgJeN6JhNCk0ov?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

Reversal payment record is created for the entry. The entry balance will update to $100 from $0

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdowNY31W1KHevvDLVY370WwLclIY2pdoU5OdOdQ-amjsHG7Yx1VATqPZCv-wwSlnNkBOixO3UX_drPFIfbkvIsrZ43XX8fuNCiOxWzFP6aaMF07rJBq-8OEI9m-bFnXIiTnesUq6ujAI55dvImN46pIhw?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>



Reversal account register record will also be created to move $100 back to account register from entry. The used and available will also be updated for the ‘Balance Refund’ that was used for entry payment



## Move Credit To Account

n the Account Tab, the 'Move Credit To Account' button will move all the credit balance present in the entry to the RP’s Account Register.



**Example: Transfer Credit Balance from Entry**

Entry ‘23191’ has a credit balance of $60.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfSIzVBTBofBQLJxLYwFNutM2lztMXkcFjqWJfjdHJ46htpeUQiWBqBjgyIS0G4k-u1e9-9Ff25tKMZ5cPNtGkWd4DEScTOW3EcaZvjszN_nGBA3svrfpACPZo6yK0A21oFWF6ZJPAvihcF3WkldQet8gh2?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>



When we transfer these $60 to RP’s Account Register:

* A payment record will be created for the entry, updating the entry’s balance from $60 CR to $0.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcoo1M_Wk3cgKXEwclQHqGSbdKANSrQvJgv_3StukBnMblmmv0UuiTvTdNnd3a1g-YpVroZ5GIOzM8CEMXsNdJsiJCWe0PkXDEOSyAz2x1oGOVxzraR4az3kTq9dqLyTHrux2BguuZhgZ9_2ukBKLH2JJlN?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

* A new Account Register record will be created for RP, and the Account Register balance will be updated to $60 CR.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXckKDRpNCYAX6X8AiWrrfdfJBvADj-Zkw7uRwzwNmOR0Ln1_ifiXgP5z_dNX3pz8augM2J8-JKvlow-Td3ugmDHYRIVrLVJ7p2IAKQkPLEHVMxcm3UUNNw_3M1Hz1aRwyJpQD8V0IqqtCAiyPu5LfqpegYS?key=rVub6YkZBoq-An-SBd1GRg" alt=""><figcaption></figcaption></figure>

