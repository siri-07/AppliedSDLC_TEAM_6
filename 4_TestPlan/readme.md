## High level Test Plan
| Test ID | Description | Exp o/p | Exp i/p | Actual o/p | Type of test |
| :---- | :---- | :---- | :---- | :---- | :---- |
| HT01 | Check functionality of the BMI and BMR calculation module | BMI 55.556, BMR 1440.00 Cal | Age 23, Height 120 cm, Weight 80 Kg, Gender male | BMI 55.556, BMR 1440.00 Cal  | Technical |
| HT02 | Check functionality of the Diet Plan and Calories intake module | Customer should be asked to plan about their diet | Customer's choice to view diet plan | Customer is asked to plan their diet | Technical |
| HT03 | Check functionality of the Water intake module | Water intake is measured for the Customer | Customer's choice to view water intake | Water intake report generated | Technical |
| HT04 | Check functionality of the Workout module | Workout plan generated | Customer's choice to view workout plan | Workout plan generated | Technical |
| HT05 | Check if the program fetches details of existing Customer | Details of Customers BMR,BMI values, Diet and workout plan should be fetched | Customer enters their ID, enters ID 0 |  Fetches all details of Customer with ID 0  | Scenario based |
| HT06 | Check functionality of the Report generation module | Report should be generated | Customer selects to generate a report and enters 2| Personalized report is generated | Scenario based |
| HT07 | Check if the program exits with proper Exit Code | Program exits | Customer wishes to exit then he/she enters 3 | Program exits | Technical |


## Low level Test Plan
| Test ID | Description | Exp o/p | Exp i/p | Actual o/p | Type of test |
| :---- | :---- | :---- | :---- | :---- | :---- |
| LT-1.1 | Check if Customer is able to choose between Imperial and SI unit system | SI system | Selects 1 | Data in SI system | technical |
| LT-1.2 | Check if Customer is alerted when height or weight exceeds the limit given | Inconsistent Data | Weight 1200kg | Inconsistent Data| technical |
| LT-1.3 | Check if Customer falls under correct weight category for BMI index | Overweight | 28 | Overweight| technical |
| LT-1.4 | Check if Customer is able to choose gender | Female | Selects 1 | Female| technical |
| LT-1.5 | Check if Customer is alerted when weight or height exceeds limit | Inconsistent Data | Weight 1200 kg | Inconsistent Data| technical |

