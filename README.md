# HDFC-Micro-Skill-Program-For-Business-Analysis
Problem Statement
The management at HDFC Bank have no means of comparing their performance in the debit and credit cards segment with industry. This is posing difficulty in strategic-planning and decision-making.

Help them by creating a dashboard to show how well HDFC performed as compared to other top banks in the Indian banking sector.
We have gathered dataset from the official site of RBI from the month of April,2022 to March,2023.
Problems in Current Structure
Some problems with data in the current form are mentioned below:
As the leadership is just interested in credit and debit cards, you need to strip irrelevant data.
There are merged cells that will cause problems when building the dashboard.
Bank names are currently clubbed depending on the bank type (public, private, etc.)
To complete this milestone, you need to clean and transform the data in all the files.
Rules to Clean Scraped Files
Here are the rules you need to follow to prepare the data for building the dashboard:
Delete columns that are not related to credit or debit cards.
Unmerge merged cells.
Aggregate "Volume" and "Value" for all the transaction modes (PoS, Online, Others.) "Value" should be in ₹ and NOT in ₹ '000s. Do not consider "Cash Withdrawal."
Remove "Payment" and "Small Finance" banks. Tag the remaining banks as "Public, Private, and Foreign."
Delete any empty rows or columns.
This Should be the structure of dataset after the cleaing process
Column
Definition
Rule
Test Value
1
bank_name
Name of the bank
NA
BANK OF BARODA
2
bank_type
Bank type: Public, Private, or Foreign
NA
Public
3
credit_cards
Total credit cards at the end of the month
NA
1194104
4
debit_cards
Total debit cards at the end of the month
NA
75272375
5
cc_transactions
Total transactions done using credit cards in the month
PoS + Online + Others
25,55,872
6
cc_inr_value
Total spending in ₹ using credit cards in the month
(PoS + Online + Others) * 1000 if given in ₹ '000s
₹ 9,28,86,60,973
7
dc_transactions
Total transactions done using debit cards in the month
PoS + Online + Others
1,27,19,853
8
dc_inr_value
Total spending in ₹ using debit cards in the month
(PoS + Online + Others) * 1000 if given in ₹ '000s
₹ 22,94,92,77,690
 Now that we have prepared the data, let's create the dashboard. But before that, remember what the leadership has asked for.

They should be able to view the performance of any bank.They should be able to compare their own bank's (HDFC) performance with the industry.

Keeping in mind the above two points, your dashboard should:

Give a high-level view of the performance of the selected bank. Show the latest numbers for both market share and KPIs and track month-on-month (MoM) growth. Give the option to select month, card type, and bank.Go into more detail:Show the overall market share number as well as the trend. Give the option to select month, card type, and bank.Show KPIs trend. Give the option to choose the bank, month, card type, and KPI. Based on the selection, show the top banks.

