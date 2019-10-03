---
layout: post
title: "Lab 5: Data Modeling"
date: 2019-10-3 22:10:38
author: "Andrew Eveld"
---
In this lab, some assumptions I had to make to design this ER and Vertabelo diagram is that
the 5% that will be given to the auction company will be figured out through
SQL queries. I also made an assumption that the auction company would not need to
be represented in the models.

<img src="https://andreweveld.github.io/csci340blog/Auction.png"/>

<img src="https://andreweveld.github.io/csci340blog/vertabelo_auction-2019-10-02_23_16.png"/>

My ER diagram from draw.io shows the suppliers having a sell relationship with
the items, but whenever I made the diagram in Vertabelo I realized it would be
simpler to attach the sell relationship from the suppliers to the bids, which
is what I did in the Vertabelo model. The highest bid will be the bid id that
gets associated with the supplier's sell. This id will be used to access the price
of the bid and other information about the bid.

Customers with certain customer IDs make as many bids as they want on the items.
Each bid holds the id of the customer that posted the bid and the id of the item
that the customer bid on. 
