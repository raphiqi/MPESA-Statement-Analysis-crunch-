**THE GOAL**

The goal of this analysis is to develop a comprehensive credit scoring system for individuals based on their M-Pesa transaction history. By leveraging various transaction-related features, such as completion time, transaction status, withdrawal patterns, and negative balances, the project aims to assess the creditworthiness of users.

**a.) What is it?**

The mission is to make borrowing money a bit fairer and more understandable for everyone. We're working on a system that looks at how people handle their M-Pesa transactions, like paying bills or sending money, to help businesses decide if they can trust someone to pay back a loan. Specifically, we're thinking about how this can benefit groups like SACCOs, making it easier for them to know their customers better.

**b.) What is it solving?**

Sometimes, the usual credit scores miss the whole picture of how someone manages their money day-to-day. We noticed that there's a need for a system that sees people's financial lives more like stories, not just numbers. Especially for groups like SACCOs, who want to lend money wisely, understanding these stories is super important.

**c.) What is the main objective?**

To create a system that gets how people really handle their money, especially when it comes to M-Pesa. We want to help businesses, like SACCOs, understand their customers beyond just a credit score – more like getting to know someone's financial story and a point of service certification for those with credible scores for loans so as to be used in other institutions.

**d.) Specific Objectives**

We want to make a credit score that looks at things like paying on time, how often someone makes transactions, and other money habits. Customize for SACCOs or other financial institutions
We're making sure our system fits right in with how SACCOs work, so they can use it easily and it matches what they need. Give Useful Info to Businesses:
We're not just about numbers. We want to give businesses info they can actually use, so they can really understand how their customers handle money.

**e.) How is the design?**

- Data Collection
- Data Cleaning
- Feature Engineering
- Modeling and visualization
- Analysis
- 
**DATA COLLECTION**
  
The data comes from MPESA Statement is derived from USSD Code *334# for a month. Since the data came in form of a PDF data had to be converted to CSV format using the link https://products.groupdocs.app/conversion/pdf-to-csv which also due security purposes enables you to insert passcode given once downloaded the statement as an OTP code.

- Load the the MPESA Statement data into the variable.
- Importing the libraries.
- Load CSV file into a dataframe.
- Load the data types of each column in the dataframe.

**DATA CLEANING**

- Replace the withdrawn column missing values with '0'.
- Convert 'Completion Time' with corrected format of datetime.
- Convert 'Withdrawn' and 'Balance' to numeric (remove commas and convert to float).
- Encode 'Transaction Status'.

**FEATURE ENGINEERING**

- Create a new column for transaction date.
- Plotting the transaction frequency per day.
- Create a new column for transaction week.
- Plotting the transaction frequency per week.
- Function to categorize transaction types based on keywords
- Average for each transaction.
- Time of day analysis.
- Occurence of negative balance.

**THE MODEL**
Used both **Decision Tree model** and **Naive Bayes model** to give a variety of options for results and they were conclusive.
