<h1 align="center"> Desafio02 </h1>

create table tbCleaner

( CLEANER_ID float primary key,

CLEANER_NAME varchar (50),

CLEANER_CPF varchar (11),

PRICE float,

CLEANING_TODAY bit(1));



create table tbHead

( HEAD_NAME varchar (50),

HEAD_CPF varchar (11) primary key);



create table tbResidence

(RESIDENCE_ID float primary key,

CITY varchar (50),

HOOD varchar (50),

STREET varchar (100),

COMPLEMENT varchar (50),

RESIDENCE_NUMBER float,

SIZE varchar (1));



create table tbCleaning

(CLEANING_ID float primary key,

`DATE` date,

CLEANING_DONE bit(1),

CLEANER_MISSED bit(1),

FEEDBACK longtext NULL);



create table tbPrice

(PRICE_SIZE float primary key);




insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (1111,'Meredith Palmer','12345678918',75.90,1);

insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (1212,'Angela Martin','11112711111',100.00,1);

insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (2718,'Andy Bernard','98745612308',55.50,0);

insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (9999,'Cathy Simms','00365847152',210.00,0);

insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (2004,'Roy Anderson','84622468157',125.00,0);

insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (3377,'Erin Hannon','42659710782',110.10,1);

insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (1234,'Ryan Howard','36952814700',89.90,0);

insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (4321,'Holly Flax','49584184636',205.00,1);

insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (4002,'Pete Miller','69420777422',99.99,1);

insert into tbcleaner (cleaner_id, cleaner_name, cleaner_cpf, price, cleaning_today)

values (8922,'Deangelo Vickers','32152298776',80.50,0);




insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (5555,'New York','Brooklyn','St. 01','A',123,'s');

insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (1010,'Los Angeles','Queens','St. 14','B',441,'m');

insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (7172,'San Francisco','Brooklyn','St. 22','B',901,'b');

insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (2332,'Seattle','Midtown','Av. 08','B',911,'b');

insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (9510,'Scranton','Midtown','St. 01','A',236,'s');

insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (7890,'Scranton','Brooklyn','St. 16','C',246,'s');

insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (3691,'Seattle','Upper East Side','Av. 12','A',555,'m');

insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (2468,'Seattle','Harlem','Av. 12','A',101,'b');

insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (7411,'Chicago','Upper West Side','St. 02','B',753,'m');

insert into tbresidence (RESIDENCE_ID, CITY, HOOD, STREET, COMPLEMENT, RESIDENCE_NUMBER, SIZE)

values (2956,'New York','Harlem','St. 14','A',772,'s');




insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Michael Scoot','4002892214');

insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Pam Beesly','88776655544');

insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Karen Filippelli','95123874601');

insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Stanley Hudson','84571296325');

insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Dwight Schrute','33628854711');

insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Robert California','02245896175');

insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Jim Halpert','15212316845');

insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Darryl Philbin','25896314470');

insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Phyllis Vance','01058874412');

insert into tbhead (HEAD_NAME, HEAD_CPF)

values ('Nate Nickerson','03629598715');




insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (1551,"2022-07-03",1,1,"Amazing job, I really recommend, five stars!");

insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (1158,"2022-07-08",1,1,"Pretty good job, 5 stars!");

insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (9877,"2022-07-13",0,0,"The cleaner did not come today >:( ");

insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (7521,"2022-07-12",1,1,"Awful job, I expected more, zero stars!");

insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (2654,"2022-07-02",1,1,"Good job, I really appreciated it, five stars");

insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (2469,"2022-07-06",0,0,"The cleaner missed the day");

insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (4200,"2022-07-03",0,0,"I'm still waiting for the cleaner, I do not recommend");

insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (3693,"2022-07-14",1,1,"Good job, but it could be better, four stars!");

insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (8488,"2022-07-12",1,1,"Bad work, I do not recommend, 0 stars!");

insert into tbcleaning (CLEANING_ID, `DATE`, CLEANING_DONE, CLEANER_MISSED, FEEDBACK)

values (1354,"2022-07-19",1,1,"Amazing job, one hundred millions stars!");




select cleaning_today,

if(cleaning_today = 1, "Yes", "No") as "Already Cleaned Today?"

from tbcleaner;



select cleaning_done,

if(cleaning_done = 1, "Yes", "No") as "Will Recieve the Payment?"

from tbcleaning;



select cleaner_missed,

if(cleaner_missed = 1, "Yes", "No") as "The Cleaner came?"

from tbcleaning;



select residence_id, size,

if(size = 's', Price from cleaner) as "Payment by Residence Size"

else if(size = 'm', Price * 2 from cleaner) as "Payment by Residence Size"

else if(size = 'b', Price * 3 from cleaner) as "Payment by Residence Size"

from tbresidence;
