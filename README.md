## Description
This challenge focuses on converting data from a reporting format back to a tabular structure format to facilitate ease of use for visualization and other general purposes. It utilizes public reporting data from the Bank of Thailand (BOT).<br>

## Objective
Often, data needs to be sourced from web scraping or various online sources, which may present in diverse formats, predominantly in a reporting layout. For instance, the sample data obtained from BOT are in an Excel reporting format, characterized by a pivot structure with hierarchy, subtotals, and total lines. Transforming this data back into a line-by-line format with proper sequencing and granularity poses a significant coding challenge.<br>

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
Using Python code within Jupyter Notebooks, we leverage Pandas and NumPy for data manipulation. The data is categorized into four groups (tables) as follows:<br>

1.Volume and Value of Plastic Card Usage - Categories: MonthYear, MeasureName, ChannelType, TransType, UsageType, M_Value. [View Code](https://github.com/chayaphon/Data_Wrangling/tree/main/Wrangling_Code/data_cleansing_Pastic_cards_usage.ipynb)<br>
2.Mobile & Internet Banking - Categories: MonthYear, MeasureName, ChannelType, TransType, SystemType, M_Value. [View Code](https://github.com/chayaphon/Data_Wrangling/tree/main/Wrangling_Code/data_cleansing_Mobile_internet_banking.ipynb)<br>
3.PromptPay - Categories: MonthYear, MeasureName, ChannelType, TransType, M_Value. [View Code](https://github.com/chayaphon/Data_Wrangling/tree/main/Wrangling_Code/data_cleansing_PromptPay.ipynb)<br>
<br>
Each transaction is identified either by volume or value under the MeasureName category.<br>
<br>

### Output data:
The data wrangling process transforms data from an Excel reporting format back to a tabular format, saving the output as .csv files in the Clean directory.<br>
[Pastic_cards_usage_Clean](https://github.com/chayaphon/Data_Wrangling/tree/main/Clean/Pastic_cards_usage_Clean.csv)<br>
[Mobile_internet_banking_Clean](https://github.com/chayaphon/Data_Wrangling/tree/main/Clean/Mobile_internet_banking_Clean.csv)<br>
[PromptPay_Clean](https://github.com/chayaphon/Data_Wrangling/tree/main/Clean/PromptPay_Clean.csv)<br>

### Simple Static Visualization by Matplotlib:
Visualizations are created using Matplotlib, as shown in the following notebooks and output images.<br>
[Matplotlib Coding Notebook](https://github.com/chayaphon/Data_Wrangling/tree/main/Visualization/matplotlib.ipynb)<br><br>
![Image](https://raw.githubusercontent.com/chayaphon/Data_Wrangling/main/img/output1.png)<br>
![Image](https://raw.githubusercontent.com/chayaphon/Data_Wrangling/main/img/output2.png)<br>
![Image](https://raw.githubusercontent.com/chayaphon/Data_Wrangling/main/img/output3.png)<br>

<hr>

### License
[Educational Purpose License](https://github.com/chayaphon/Data_Wrangling/blob/main/LICENSE.md)

### Written By
- **Name**: Chayaphon Sornthananon
- **Email**: s_chayaphon@outlook.com
