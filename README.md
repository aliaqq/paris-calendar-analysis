# paris-calendar-analysis
A Python project that uses the calendar module to analyze a Paris dataset, focusing on monthly and seasonal trends.
## for the following analysis i have downloaded the data from : https://data.insideairbnb.com/france/ile-de-france/paris/2024-09-06/data/calendar.csv.gz

``` diff
import pandas as pd

data = pd.read_csv('calendar.csv')
```
## to know number of available and unavailable rooms
<img width="305" alt="Screenshot 1446-07-19 at 2 45 23 PM" src="https://github.com/user-attachments/assets/51075729-69d6-40a7-9a7f-f30fd27f9469" />

## 2
diff
df['available'].value_counts(normalize=True)

## 3
diff
busiest = df[df['available']=='f']['date'].value_counts()
print(f'Busiest Dates: {busiest.head()}')




