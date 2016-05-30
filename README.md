# SQLite


// 删除表

drop table person;

// 创建表

create table person(id integer primary key autoincrement, name varchar(20), sex smallint, age smallint, email text, address text, tel text);

// 插入数据

insert into person values(null,'tom',0,101,'tom@126.com','beijing','15253208570');

insert into person(name,sex,age,email,address,tel) values('jhon',1,36,'john@163.com','上海','18566325689');
insert into person(name,sex,age,email,address,tel) values('dream',0,48,'dream@hotmail.com','广州','13553211314');

insert into person(id,name,sex,age,email,address,tel) values(null,'william',0,48,'william@sogou.com','深圳','17213145215');


// 更新数据

update person set address = '北京' where name = 'tom';

// 删除数据

delete from person where name='tom';

// 查询数据

select * from person ;

select * from person where name = 'john';
