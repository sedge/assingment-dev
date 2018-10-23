# Assignment - MapReduce

Write an map-reduce engine that can execute programs according to the map-reduce paradigm.
Provide two endpoints using your engine with an architecture that can easily beeing extended.
Test the functionality with at least one test each.

First endpoint counts the transaction of a merchant. 

In:

transactions
Out:

merchant_transaction_count: [starbucks:3,Tim Hortons: 4]

Second endpoint combines the transactions with the users and calculates the percentage of good reflections for each user name.

In: 

transactions, users

out:

user_happiness: [{John:50%}, {Luke:100%}]



Transactions:

```Javascript
transactions: [
{id:1, merchant:starbucks, amount:1.78, date:2018-01-01, reflected:GOOD, user_id: 1},
{id:2, merchant:starbucks, amount:5.76, date:2018-01-02, reflected:GOOD, user_id: 1},
{id:3, merchant:Tim Hortons, amount:8.76, date:2018-01-03, reflected:NEUTRAL, user_id: 1},
{id:4, merchant:Tim Hortons, amount:5.67, date:2018-01-04, reflected:BAD, user_id: 1},
{id:5, merchant:Tim Hortons, amount:11.76, date:2018-01-06, reflected:GOOD, user_id: 1},
{id:5, merchant:Starbucks, amount:12.36, date:2018-01-07, reflected:GOOD, user_id: 2}
{id:5, merchant:Tim Hortons, amount:1.45, date:2018-01-08, reflected:GOOD, user_id: 2}
]
```
Users:
```Javascript
users: [{id:1, name: John},{id:2, name: Luke}]
```
