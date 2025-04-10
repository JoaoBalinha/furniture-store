# Furniture-store
## Hi there! 
 So, I’m learning Python and starting to give my first steps at this language. 
 I’m going to start by presenting you a few simple things that this language can do for us.
 As an example, I’m going to use a fiction dataset about a furniture store and their stock.
 I’m going to star be doing some simple things and then, get a little more difficult as we’re going along this journey. 
Our dataset will have a few items and what we want to do is things like:

## Create a program that asks the user for the price of 5 pieces of furniture and calculates the total value of these items. Use a loop to handle data input. 
	Simple Variables
```{python}
import pandas as pd

furniture = "Bed", "Sofa", "Table"  # Idenitfy the pieces
price = 600, 400, 300  # How much each one cost
stock = 17, 23, 12  # How much stock we have

print(f"Furniture: {furniture}, Price €{price}, Stock: {stock}")
```
  	Variable Type
    o	Ask the user for the name of a piece of furniture, its price, and the quantity in stock using input. Identify the data type for each variable.
```{python}
furniture = input( "What kind of furniture are you looking for: ")
price = input("How much does it cost: ")
stock = int(input("How much stock do you have: "))

# Print type of variable
print(f" The type of {furniture} is, {type(furniture)}")
print(f" The type of {price} is, {type(price)}")
print(f" The type of {stock} is, {type(stock)}"
```
	Simple Conditional
```{python}
question = input("Pretend to purchase this furniture? Yes or No:")

if question.lower() == "Yes":
    print(f"Your order has been placed ")

else:
	  print("The item is still available")
```
## Ask the user if they want to buy a piece of furniture. If they answer "yes," display a message saying that the furniture has been reserved; otherwise, inform them that it remains available.

	Compound Conditional
```{python}
```
## Ask the user for the price of a piece of furniture. If the price is greater than 1.000,00€, display "Premium product"; if it is less than or equal to 500,00€, display "Economical product". For other cases, display "Intermediate product".

	Loop with Counter
```{python}
price = float(input(" Please specify the price of the item: "))
if price > 1000:
	              print("Premium Product")
elif price <= 500:
	              print("Economic Product")
else:
	              print("Intermediate Product")
```
## Display a 5-second countdown to announce a discount on furniture

	Loop with User Input
```{python}
for number in range(5, 0,-1):
    print(f"Discont in {number} seconds... ")
print("Descont activated")
```
## Create a program that allows the user to add furniture to a shopping cart. The program should stop asking for inputs when the user types "exit."

	List Comprehension
```{python
price = [2000, 750, 1200, 350]

price_with_descont = [price*0.9 for preco in price]

print("Price with 10% descont", price_with_descont)
```  
## Suppose the store has a list of furniture prices. Create a new list with prices discounted by 10% using list comprehension.

	Slice
```{python}
furniture = ["Sofa", "Table", "Chair", "Rack", "Bed"]

print("The first three", furniture[:3] )
print("The last two", furniture[-2:])
print("Price with 10% descont", price_with_descont)
```
## Consider a list of furniture on sale: ["Sofa", "Sideboard", "Chair", "Rack", "Bed"]. Show the first 3 and the last 2 items of the list.

	Loop with Conditional
```{python}
prices = [1200, 850, 300, 500, 1500] # Price range

for price in prices:
  if price > 1000:
    print(f"Price above 1000: {price}")
```  
## Given a list of furniture prices, display only the prices that are greater than a specified value. Example: prices = [1200, 850, 300, 500, 1500].

	Challenge: Sum of Values
```{python
total_value = 0

for i in range(5):
	  price = float(input(f"Tell the price {i+1} furniture: "))
	  total_value += price

print(f"Furniture total value: {total_value} €")
``` 




