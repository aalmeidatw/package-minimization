#Package Minimization

## Introduction 

An electronics company is planning to sell their products worldwide. In order to supply the new demand, the company is going to create multiple distribution centers around the world.

An optimized profit can be achieved by reducing the shipping cost. Every time a distribution center cannot fulfill an order completely, more than one package will be delivered to the customer and the shipping cost will be increased.

Consider an example which an order has been placed with the items below:

| Product  | Quantity | 
| -------- | ---------|
| Keyboard |        1 | 
| Monitor  |        1 | 

Also, the following distribution centers have the products available:

| Center | Product  | Quantity | 
|------- | -------- | ---------|
| Brazil | Keyboard |        2 | 
| Chile  | Monitor  |        3 | 

The result would be two shipments, one package from Brazil with the keyboards and another package from Chile with the monitors.

## Problem

The purpose of this problem is to fulfill the order with the minimum possible number of packages. In other words, the result should be the best combination of distribution centers that have the products available in the required quantities.

*Note: in case of a tie between two distribution centers, both responses are acceptable.*

The input is separated by two parts, the first one is the list of distribution centers and the products available in each one of them. The second part is the order that need to be fulfilled using the loaded availability from the first part. 

The output is the number of packages followed by the list of distribution centers that will fulfill the order with the product and quantity		

### Test Example

#### Input

    Brazil Keyboard 2
    Brazil Mouse 1
    Brazil Monitor 1
    Chile  Keyboard 2
    Chile  Monitor 2
    Panama Mouse 2
    Argentina Monitor 2
    Keyboard 3
    Mouse 1
    Monitor 2

Basically, in this example, the last three lines represent the order because they don't have any distribution center associated to them.

#### Output
	2
    Brazil Keyboard 2
    Brazil Mouse 1
    Brazil Monitor 1
    Chile  Keyboard 1
    Chile  Monitor 1

Even though the output has multiple lines, there are just two packages, one from Brazil and another one from Chile.
