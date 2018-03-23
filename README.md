# ica4

## Question 1
How many people search for a host on Airbnb every day during first week 2014?

```sql
select 
ds,
count (Distinct id_user) as count
From strata_user.airbnb_sq
where ds>='2014-10-01'and ds<='2014-10-07'
group by ds
```

|[ica4](visualize/graph.jpg)
