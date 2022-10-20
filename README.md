# ROIcollections

This project let us see the return on investment on several collections based on their staking rewards and their floor price.

We grab informations from :
1. MagicEden API for floor prices of collections
2. CoinMarketCap API for token price
3. A .xlsx file giving the collection name (for ME API), the token name (for CMC API), the quantity of tokens per day.

![image](https://user-images.githubusercontent.com/112710446/196964149-6d0f3e06-e597-4408-9897-84667a488cf5.png)

Then I clean the datas, make it all in one database, run a few calculations and export the result in another .xlsx file.
I then use the .xslx file in Tableau Public to get this dashboard :
https://public.tableau.com/app/profile/kano/viz/ROIDays/Dashboard1

![image](https://user-images.githubusercontent.com/112710446/196965733-ced701d9-92b1-43b0-b585-02773d81c53d.png)

Could be improved : 
* Find a way to get the liquidity of each tokens.
* Find a way to filter floor with attributes (for example turtles staking reward is different for gen1 and gen2).
* Host the imported .xlsx on google sheets
* Host the exported .xlsx on google sheets
* Find a way to run the script by itself every day and host it on web
