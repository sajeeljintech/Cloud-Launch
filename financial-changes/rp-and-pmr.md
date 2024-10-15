---
icon: users-between-lines
---

# RP & PMR

## PMR Change



#### **Example 1: Prize Money not applied and PMR is changed**

If no prize money is applied and PMR is changed, then we will simply change the entry’s PMR and nothing more.

#### **Example 2: Prize Money is applied and PMR is changed**

If prize money is applied and PMR is changed, then all the applied prize money to the current entry will be rolled back. Prize Money rollback test cases are discussed in the rollback section.

#### **Example 3: Prize Money is applied and old or new PMR is foreigner**

If prize money is applied and either the old or new PMR is a foreigner, then the PMR will not be changed. Instead, the PMR source will be changed to 'Others', if it is not already 'Others'.

## RP Change

f the entry’s RP is changed, then all the balance refunds transferred to the Account Register (by cloud) from the current entry will be rolled back.

#### **Example 1: No Balance Transferred to A/R and RP is changed**

If no balance refund is transferred to A/R and RP is changed, then we will simply change the entry’s RP and nothing more.

#### **Example 2: Balance Transferred to A/R and RP is changed**

If a balance refund is transferred to A/R by current entry and RP is changed, then we will move the credit back from A/R to the entry before changing the entry’s RP.

#### **Example 3: Balance Transferred to A/R and used for multiple entries payoff, then RP is changed**

If a balance refund is transferred from current entry to A/R and used for entries' payoff, and then RP is changed, then:

* All payments made to entries by that amount will be reversed.
* The amount will be transferred from A/R back to the entry.
* Then, RP will be changed.

#### **Example 4: Balance Transferred to A/R and check is paid**If balance refund was transferred to A/R by current entry and then it was used for RTO check payment, then:

* Check paid by balance refund will not be reversed.
* But, the Balance Refund moved to A/R will be moved back to the entry.
