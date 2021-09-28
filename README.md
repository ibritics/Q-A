# Q/A
## Python
**Question: Convert the price to a float. The price column currently contains strings with the ‘$’ symbol and commas. For example $1,200. Here is a super quick way of converting the entire column to float values.**
<br /> Answer: <br />
```
data['price']=data['price'].apply(lambda x: locale.atof(x.strip("$")))
```
