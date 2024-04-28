# Python-Challenge-1

I worked with tutor Mohammed Fauwaaz in a Tutor Session on BSC to complete this assignment.

## Overview
Use the starter code provided for printing a menu for the customer, create an ordering system to allow the customer to place an order, store the order and printing the receipt with the total price of all items ordered.

## Purpose
Utilize print statements, loops, dictionaries, lists, list comprehension and if-else statements to navigate through the menue options, storing menu, and calculate the total order price.

## Business Advantage [^1]

![Food_Truck_POS](images/Food_Truck_POS.jpeg)

In order to meet to demand of customer on-the-go, the food truck business requires vendors to mobile, prepared, and organized to order to maximize opportunities and sales. A big part of this involves have a POS system that allows customers to place orders, pay, and receive a receipt. This kind of system is need to run and grow and food truck business.

## Landscape
Point of Sales (POS) are an essential part of the food truck business. Here are five benefits to POS system:
1. Ability to take payments anytime and anywhere
2. Ease of tracking sales and revenue based on products, and location and time, which helps with future inventory
3. Increased efficienty and accuracy in a chaotic business
4. Managing inventory throughout the day through simple reports from the dashboard to show how many items were sold, and providing the ability to reorder   ahead of time for next shipment.
5. Build a customer database for marketing by providing customer with a way to enter emails and phone numbers for direct marketing and texting campaigns.

## Results

### Order System: 
- Order list was created to store list of dictionaries for menu item name, item price, and quantity. Starter code with while loops, for loops, and if-else statements provided to print menu_items dictionary (A dict of the key:value pairs for menu item numbers 1-4 and the corresponding menu categories: Snacks, Meals, Drinks, Desserts), prompt customer to order from menu_items, check to ensure customer order for menu_category is a integer and valid option in menu_items dict, print the menu category name associated with menu item number selected, prints menu_category_name options from sub-level menu_items dict. (1)
- Prompted user to input menu item number from the menu_items dict, store input as menu_selection, check to ensure customer menu_selection is a integer and valid option in menu_items dict. Item name stored as variable menu_item_name. Prompt customer to enter the quantity of menu_item_name and save input to variable quantity. Input for quantity checked to ensure was integer. Customer's order appended to empty order list as a dictionary with the following keys: "Item name", "Price", and "Quantity". (2-4)
- While loop created to prompt customer to enter "y" or "n" regarding whether they want to continue ordering, with match:case statements created to check for "y" to set the place_order variable to True and break from the "keep ordeing question" loop, check for "n" to set place_order variable to False to print "Thank You for your order" and break from the continuous while loop, or default and tell customer to try again because they didn't type a valid input.(5)

### Order Receipt:
- For loop created that iterates over the sequence of numbers starting from '0' and ending at 'len(order_list) - 1', with x representing each iteration, and x taking on the value of the current number in iteration sequence. Value for each key saved to it's own following variable: item_name, price, and quantity. (6-7)
- Format receipt by calculating number of empty spacesto display based on provided receipt format, create space strings using their respective variables and sting multiplication, and print each line of receipt using the provided format. (8-10)
- Total price of order calculated and displayed to customer, once loop is exited, by getting the sum() of a list comprehension used to multiply the price by the quantity for every item in the order list. (11)

## Recommendations
Application should also prompt user to enter email and phone number to build a customer database for direct marketing, texting campaigns, social medica engagements, and rewards or loyalty programs.

[^1]: https://www.appstar.net/5-reasons-every-food-truck-needs-a-pos-system/
