#projects/united-journal/services

*Who/what/when/where/why/how breakdown followed by features and other notes.* 
# Breakdown

### Who?
Customers and the Lansing team.

### What?
Long story short, it would be a wrapper for orders. You could group orders together, schedule partial material pickups/deliveries, keep track of ongoing cost and labor, manage warranties, break down bulk pricing and rebates.
### When??  Where ???
### Why?
The idea for this service originally came from dealing with one of our customers who has several ongoing apartment jobs/bids. He is ordering such a large quantity of material, having to schedule weekly deliveries or coordinating with his crew to pickup almost daily. It is a lot of work to have to go through each order and allocate materials for a small pickup. We end up having to take from a different building when the supplier falls behind on production, which ends up messing up total material counts in the end. 

It sums up to the Lansing team doing a lot of extra work that could be handled with a wrapper around the order system.

- It is intended for our management of the ongoing project. It would also be a great tool for our customers to generate quotes for their customers, manage other costs of products, and help us gather more intelligence on where they are buying materials. 
### How?
The simplest answer, a wrapper around the current order implementation. The order system can remain the same. 

**Solution \#1:** ***Control Via Master Order***
- Control via a master order works by making one order for the total material for a section of buildings using the same material.
- When a deliver, pickup, or the next phase of the is required, the project service creates a new order and allocates material from the master order to the child order. 


**Solution \#2:** ***T***


# Features 
### Customer Features
- Help break down and understand costs of projects. (Material, labor, lead times, cost of one material vs another.)
- Generate quotes for their customers
- \*\*Track invoices from other suppliers. Think of #projects/in-gen-man, it would be a great external API integration. I would not imagine the customers are willing to share invoices from other suppliers with Lansing.

### Lansing Team Features
