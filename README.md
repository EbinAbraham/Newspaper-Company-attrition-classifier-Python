Newspaper Company attrition classifier-Python

==================================================================================

<h1>Newspaper Company Attrition Classification</h1

==================================================================================

<h3>Overview</h3>

The objective of this project is to determine which customers will churn. Thus the company can predict the number of subscribers and also provide offers to the customers who may churn so as to retain them. The dataset was obtained from a private repository hence not uploading the dataset.

==================================================================================

<h3>Dataset</h3>

The dataset contains 5 text files which were merged together to obtain the final dataset on which the analysis was done. After merging there were 27 columns, details of this is given below.



| __Feature__       | Description                                                  |
| ----------------- | ------------------------------------------------------------ |
| Subscription Id   | Unique Subscription identifier                               |
| DeliveryType      | Type of delivery                                             |
| DeliveryClass     | Delivery is normal or abnormal                               |
| StartDate_x       | Start date delivery                                          |
| EndDate_x         | End date delivery                                            |
| CustomerID        | Customer Identifier                                          |
| ProductID         | Product Identifier                                           |
| Pattern           | Denoted Delivery Days                                        |
| StartDate_y       | The subscription start date                                  |
| EndDate_y         | The subscription end date                                    |
| NbrNewapapers_x   | Total number of copies                                       |
| RenewalDate       | Date on which renewal is processed                           |
| PaymentDate       | Date of payment                                              |
| PaymentType       | BT = Bank Transfer<br>DD = Direct Debit                      |
| PaymentStatus     | Paid or not paid                                             |
| FormulaID         | Formula Identifier                                           |
| NetNewspaperPrice | Price of a single newspaper                                  |
| ProductDiscount   | Discount based on product                                    |
| FormulaDiscount   | Discount based on formula                                    |
| TotalDiscount     | Total discount=ProductDiscount+FormulaDiscount               |
| TotalCredit       | Customers credit of previous transaction. Credit is negative and debit is positive |
| Gender            | Male or Female                                               |
| DOB               | Date of birth                                                |
| District          | District of residence                                        |
| ZIP               | Zip code                                                     |
| StreetID          | Street Identifier                                            |
| Churn             | Whether customer has left the service                        |

 

==================================================================================

<h3>Proccessing</h3>

Initially individual text required cleaning of data to appropriate columns. Missing value were handled using mode, median and creating new category for unknow. Outliers were capped for obtaining good solution. Time stamp data were converted to ordinal for processing. Moreover categorical variables were label encoded.

==================================================================================

<h3>Result</h3>

Two models were created logistic regression and random forest. Based on the output provided random forest classifier was adjudged the better model. The details are as follows

__Confusion Matrix__

[[3396   19]

[  33 1343]]

| __Metric__              | Value              |
| ----------------------- | ------------------ |
| Cross Validation Score  | 0.988310746868714  |
| Testing Accuracy        | 0.9891463160091839 |
| F1 Score                | 0.9810080350620891 |
| AUC                     | 0.98522687612789   |
| Average Precision Score | 0.9692898417262321 |

==================================================================================