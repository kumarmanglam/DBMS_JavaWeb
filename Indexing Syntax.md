
```sql
use first;
create table second_table (
	id int not null auto_increment,
	fname varchar(20),
    age int,
    primary key (id)
);

select * from second_table;

insert into second_table (id, fname, age) values (8, "Jaya", 85);

CREATE INDEX age_index ON second_table (age);

SELECT * FROM second_table WHERE age > 50;
```

