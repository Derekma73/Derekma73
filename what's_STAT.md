A great question! Here are some notes on what STAT is, as according to notes made on 9/20/2018. 

* STAT is the calculation of voting power that affiliates have during convention and the amount of dues that each one pays. 

## The Steps 
* Per Capita System - The raw data as entered by Accounting. 

* Preliminary STAT - The data calculated from Per Capita System. 

* Final STAT - Generally the same as Preliminary STAT, but gone through the vetting process again to make sure it's correct. Generally will use this over the other two. 

## STAT Schema 
There are several tables, but only six of the tables within the schema are useful. 

* `audit_items` - The equivalent of per capita system, essentially the raw data. 

* `stat_local` - Information on locals. Those without a parent local are associated with the IU.

* `stat_payment` - The preliminary stat.

* `stat_local_avg` - The equivalent of the final stat calculation - based on 
audit_items/stat_payment. This is typically what you'll be pulling from. 

* `audit_percap_rates` 

* `audit_distribution_codes` - Contains what the distribution codes mean within the other tables.

Supplement the code information with `enterprise_replica.common_codes`. 
