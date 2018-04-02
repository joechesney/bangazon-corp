# Bangazon Corporation

## The Personal E-Commerce Platform

Bangazon Corp welcomes you to the team. You've been selected from a deep pool of candidates to help build the next, disruptive online platform. Our goal is to become the most personalized, and most powerful commercial platform for individuals all around the globe.

You are needed to make that happen.

In order to become a profitable, and sustainable organization, we need you to build all of the technology and tooling for the company.

## Orientation

Your first three weeks on the job will be your orientation to the technical languages, tools, and frameworks that you'll be using. You will also be introduced to the processes and procedures that you will need to follow to ensure high communication and high productivity for your team.

1. Installation of required tools.
1. Introduction to the language.
1. Concepts of sustainable, scalable, object-oriented software development.
1. Test driven development
1. Overview of server-side development ecosystem
1. How the Internet works
1. Entity relationships
1. Structured Query Language (SQL)

At the end of your orientation, your management team will determine which Development Team you will be assigned to for the next three months.

## Platform Development

You will work on four different [Sprints](https://www.scruminc.com/sprint/) while you build the products that Bangazon Corporation needs in order to operate as a modern business. On each of these sprints, you will build features that your product owner has defined in the [Backlog](http://www.mountaingoatsoftware.com/agile/scrum/scrum-tools/product-backlog).

Your management team will ensure that you have the proper training in the skills, concepts, and tools needed to complete the projects, and then you will fulfill the requirements for the project until you are done, as defined in the [Bangazon Definition of Done](https://github.com/nashville-software-school/bangazon-llc/blob/master/EMPLOYEE_HANDBOOK.md#definition-of-done).


# Alternate Readme:
<!-- Review-ready -->
NODE Version:
# Bangazon

## The Command Line Ordering System

In this group project, you will be allowing a user to interact with a basic product ordering database.

## Ordering System Interface

### Main Menu

```bash
*********************************************************
**  Welcome to Bangazon! Command Line Ordering System  **
*********************************************************
1. Create a customer account
2. Choose active customer
3. Create a payment option
4. Add product to shopping cart
5. Complete an order
6. See product popularity
7. Leave Bangazon!
>
```

### Create Customer

```bash
Enter customer name
>

Enter street address
>

Enter city
>

Enter state
>

Enter postal code
>

Enter phone number
>
```

### Choose active customer

```bash
Which customer will be active?
1. John Q. Public
2. Svetlana Z. Herevazena
>
```


### Create Payment Option

```bash
Enter payment type (e.g. AmEx, Visa, Checking)
>

Enter account number
>
```

### Add Product to an Order

> **Note:** These are examples. Add your own product names, please.

To make it easier to add multiple products, when the user selects a product to order, display the menu of products again. Make sure the last option of *Back to main menu* so the user can specify that no more products are needed.

```bash
1. Diapers
2. Case of Cracking Cola
3. Bicycle
4. AA Batteries
...
9. Done adding products
```

### Complete an Order

##### If no products have been selected yet

```bash
Please add some products to your order first. Press any key to return to main menu.
```

##### If there are current products in an order

```bash
Your order total is $149.54. Ready to purchase
(Y/N) >

# If user entered Y
Choose a payment option
1. Amex
2. Visa
>

Your order is complete! Press any key to return to main menu.

# If user entered N, display the main menu again
```

Once the order is complete, show the main menu again, where the user can start creating another order.

### See Product Popularity

When selecting this option, you will produce a command line report that looks like the following.

```bash
Product           Orders     Customers  Revenue
*******************************************************
AA Batteries      100         20        $990.90
Diapers           50          10        $640.95
Case of Cracki... 40          30        $270.96
*******************************************************
Totals:           190         60        $1,902.81

-> Press any key to return to main menu
```

1. The product column must be 18 characters wide, and will display a maximum of 17 characters for the product name.
1. The orders column must be 11 characters wide.
1. The customers column must be 11 characters wide.
1. The revenue column must be 15 characters wide.

# Requirements

You will create a series of prompts that will allow the user to create various types of data in your ordering system.

1. Use the npm module `prompt` to create an interface for prompting your user for input.
1. Your team must have full test coverage for all functionality. Start with writing unit tests.
1. You must use the db you created in the earlier SQL exercise. Choose one team member's implementation to be your group's database.
1. For the Product Popularity section, search for an npm module that will output your report in table format to the console.
