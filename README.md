# SQL_Stored-Procedure

![1](https://user-images.githubusercontent.com/33677647/204162658-d0cca2ac-f133-4416-bf72-bd39ac50b7c1.jpeg)
![2](https://user-images.githubusercontent.com/33677647/204162711-a87dcf51-de83-4042-b73f-35de4b44dfde.jpeg)

Stored procedures are used to do the work that simple sql query can not do.
- It starts with the keyword "create or replace prcedure than_here_name_of_your_procedure (nameOfFirstParameter ItsDataType, nameOfSencondParameter ItsDataType)"
- then on second line, specificly in postgreSQL you have to specify that which language we will use here,<br/> because postgreSQL also supports python/c++/etc, so "language plpgsql".
tell we are using sql here.
- "as $" (it is a doulbe dollar actually) on third line and "$" at the last most line to avoid escape characters of any string error in between area.<br/>
- the procedure body, where all the logic is written is in between "begin" and "end;" keywords.
- we could have used "create procedure" only, but if we want to update an existing procedure we can use "create or replace procedure"

![3](https://user-images.githubusercontent.com/33677647/204162670-46363429-13f1-4130-a510-108f4bfc9ebe.jpeg)
