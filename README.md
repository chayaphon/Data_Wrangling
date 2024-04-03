# Description
This challenge is to clean and reverse data format fron reporting format back to tabular structure format.<br>
And so it's easy to use for various of visualization and other general purpose.<br>
This excercise will use data from BOT (Bank of Thailand) public reporting data.<br>

## Objective
Sometime we need to enquiry data from web scraping or various source of data from internet, and many of them may be came with different format or most of them came with reporting format.<br>
Like in the sample data we get from BOT as execl reporting format which are in pivot structure and with hirachy and subtotoal and total line.<br>
This is very challange to coding for reverse enginerering for getting data line by line with a proper sequence and grainulity.<br>

## Datasource
[Data](https://raw.githubusercontent.com/chayaphon/Data_Wrangling/main/Sources/Data.xlsx)<br>
[Source from Bank of Thailand](https://www.bot.or.th/en/statistics/payment.html)<br>

| Report                         | Level of Data | Range                |
|--------------------------------|---------------|----------------------|
| Vol. of Plastic card usage     |    Monthly    | Jan 2020 - Dec 2023  |
| Value. of Plastic card usage   |    Monthly    | Jan 2020 - Dec 2023  |
| Mobile, internet banking       |    Monthly    | Jan 2020 - Dec 2023  |
| promptpay                      |    Monthly    | Jan 2020 - Dec 2023  |

## Sample of Data
Vol. of Txn by Payment System/ <br>
![Image](https://raw.githubusercontent.com/chayaphon/Data_Wrangling/main/img/ss_sample.png)

## Task
### Data Wrangling and Tranformation :
We will use python code with jupytor notebooks to write the code for all tasks, we mainly use Pandas and numpy for these task.<br>
I have define the data into 4 groups (tables)<br>

[1.Volumne and Value of Plastic card usage](https://github.com/chayaphon/Data_Wrangling/tree/main/Wrangling_Code/data_cleansing_Pastic_cards_usage.ipynb)<br>
  we are going to categorize data into : MonthYear, MeasureName, ChannelType, TransType,  UsageType, M_Value<br>
[2.Mobile, internet banking](https://github.com/chayaphon/Data_Wrangling/tree/main/Wrangling_Code/data_cleansing_Mobile_internet_banking.ipynb)<br>
  we are going to categorize data into : MonthYear, MeasureName, ChannelType, TransType,  SystemType, M_Value<br>
[3.Promptpay](https://github.com/chayaphon/Data_Wrangling/tree/main/Wrangling_Code/data_cleansing_PromptPay.ipynb)<br>
  we are going to categorize data into : MonthYear, MeasureName, ChannelType, TransType, M_Value<br>
<br>
As of all transaction give both in volumes and values, so we will keep this indicator for each metrics as MeasureName (volume,value)<br>
<br>

### Output data:
The above perform data wrangling and tranforming from excel reporting format reverse back to tabular format which save output in .csv file at directory Clean.<br>
[Pastic_cards_usage_Clean](https://github.com/chayaphon/Data_Wrangling/tree/main/Clean/Pastic_cards_usage_Clean.csv)<br>
[Mobile_internet_banking_Clean](https://github.com/chayaphon/Data_Wrangling/tree/main/Clean/Mobile_internet_banking_Clean.csv)<br>
[PromptPay_Clean](https://github.com/chayaphon/Data_Wrangling/tree/main/Clean/PromptPay_Clean.csv)<br>

### Simple Static Visualization by Matplotlib:
[matplotlib coding](https://github.com/chayaphon/Data_Wrangling/tree/main/Visualization/matplotlib.ipynb)<br><br>
![Image](https://raw.githubusercontent.com/chayaphon/Data_Wrangling/main/img/output1.png)<br>
![Image](https://raw.githubusercontent.com/chayaphon/Data_Wrangling/main/img/output2.png)<br>
![Image](https://raw.githubusercontent.com/chayaphon/Data_Wrangling/main/img/output3.png)<br>

<hr>

### License
[Educational Purpose License](https://github.com/chayaphon/Data_Wrangling/blob/main/LICENSE.md)

## Written By
- **Name**: Chayaphon Sornthananon
- **Email**: s_chayaphon@outlook.com
