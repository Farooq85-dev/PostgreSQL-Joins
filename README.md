# PostgreSQL-Joins

## This repository is about the joins operation or methods in PostgreSQL.

## Joins Types:-

- Cross Join
- Left Join
- Right Join
- Inner Join or Join

### 1) `Join or Inner Join`

#### A JOIN clause is used to combine rows from two or more tables, based on a related column between them. For example:-

```
select * from customer c inner join orders o on c.id = o.customerId;
```
###### See Picture
![inner-join](./images/Screenshot%20from%202024-10-14%2011-34-08.png)


### 2) `Cross Join`

#### Every row from one table is combined with every row from another table. For example:-

```
select * from customer cross join orders;
```

### 3) `Left Join`

#### Returns all rows from the left (or first) table and the matching rows from the right (or second) table. For Example:-

```
select * from customer left join orders on orders.customerId = customer.id
```

###### See Picture
![left-join](./images/Screenshot%20from%202024-10-14%2011-34-23.png)


### 4) `Right Join`

#### Returns all rows from the right (or second) table and the matching rows from the left (or first) table. For example:-

```
select * from customer right join orders on orders.customerId = customer.id
```

###### See Picture
![right-join](./images/Screenshot%20from%202024-10-14%2011-34-38.png)