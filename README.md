# Assignment - MapReduce

Write an express app using map-reduce that can execute programs according to the map-reduce paradigm.
Provide two endpoints using your engine with an architecture that can easily be extended.
Test the functionality with at least one test each (we prefer Jest, but feel free to use whichever testing library you wish to use).

## First endpoint: counts the transactions of each merchant. 
This endpoints counts the transaction of each merchant.

```
Example Input:
transactions

Example Output:
merchant_transaction_count: [Starbucks:3,Tim Hortons: 4]
```

## Second endpoint: percentage of happiness per user
This endpoint combines the transactions with the users and calculates the percentage of good reflections for each user name.

```
Example Input: 
transactions, users

Example Output:
user_happiness: [{John:50%}, {Luke:100%}]
```

Transactions:

```Javascript
{id:1, merchant:Starbucks, amount:1.78, date:2018-01-01, reflected:GOOD, user_id: 1},
{id:2, merchant:Starbucks, amount:5.76, date:2018-01-02, reflected:GOOD, user_id: 1},
{id:3, merchant:Tim Hortons, amount:8.76, date:2018-01-03, reflected:NEUTRAL, user_id: 1},
{id:4, merchant:Tim Hortons, amount:5.67, date:2018-01-04, reflected:BAD, user_id: 1},
{id:5, merchant:Tim Hortons, amount:11.76, date:2018-01-06, reflected:GOOD, user_id: 1},
{id:5, merchant:Starbucks, amount:12.36, date:2018-01-07, reflected:GOOD, user_id: 2}
{id:5, merchant:Tim Hortons, amount:1.45, date:2018-01-08, reflected:GOOD, user_id: 2}
```
Users:
```Javascript
{id:1, name: John},{id:2, name: Luke}
```
Links:
https://en.wikipedia.org/wiki/MapReduce
