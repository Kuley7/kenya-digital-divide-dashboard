# Kenya Digital Divide dashboard (Power BI)

![Dashboard](kenya%20digital%20divide.png)
A Power BI dashboard showing **who is connected in Kenya, and who is left behind**. It uses official data from the **2019 Kenya Population and Housing Census** for all 47 counties.

## Key findings
- **Most Kenyans own a phone, but fewer than 1 in 4 use the internet.** 47.3% of people aged 3+ own a mobile phone, 22.6% use the internet, 10.4% use a computer, and only 4.3% of adults shop online.
- **A 7.6× divide between counties.** Nairobi leads at 52% internet use, while Turkana is at 7%. Nairobi, Kiambu and Mombasa lead; Turkana, Mandera, West Pokot, Wajir and Marsabit trail.
- **Urban vs rural at every age.** Among 25–34 year olds, 64% of urban residents use the internet, against 30% in rural areas. Urban areas hold 58% of all internet users.
- **The gender gap grows with technology.** Men and women own phones at almost the same rate (47.6% vs 47.0%), but for internet use the gap is 5 points (25.1% vs 20.1%).

## Dashboard contents
- 4 KPI cards: mobile ownership, internet use, computer use, online shopping
- Internet use by age, urban vs rural (line chart)
- Internet users by sex and by residence (donuts)
- Internet use for all 47 counties (bar chart; click a county to filter the page)

## Data
**Source:** Kenya National Bureau of Statistics (KNBS), *2019 Kenya Population and Housing Census*, Volumes I and IV. The tables were compiled through the open-data [rKenyaCensus](https://github.com/Shelmith-Kariuki/rKenyaCensus) package.

Data model: a `Counties` table (47 rows) related one-to-many to `Gender`, `SubCounties` and `AgeByCounty`, plus a Kenya-wide `UrbanRuralByAge` table.

## Key DAX measures
