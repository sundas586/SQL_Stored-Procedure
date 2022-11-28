# SQL_Stored-Procedure

A stored procedure is a prepared SQL code that you can save, so the code can be reused over and over again.
So if you have an SQL query that you write over and over again, save it as a stored procedure, and then just call it to execute it.
You can also pass parameters to a stored procedure, so that the stored procedure can act based on the parameter value(s) that is passed.

![1](https://user-images.githubusercontent.com/33677647/204250061-8001eab2-f5d5-43df-a7b7-0aa1a445ea76.JPG)
![1](https://user-images.githubusercontent.com/33677647/204162658-d0cca2ac-f133-4416-bf72-bd39ac50b7c1.jpeg)
![2](https://user-images.githubusercontent.com/33677647/204162711-a87dcf51-de83-4042-b73f-35de4b44dfde.jpeg)

Stored procedures are used to do the work that simple sql query can not do.
- It starts with the keyword "create or replace prcedure than_here_name_of_your_procedure (nameOfFirstParameter ItsDataType, nameOfSencondParameter ItsDataType)"
- then on second line, specificly in postgreSQL you have to specify that which language we will use here,<br/> because postgreSQL also supports python/c++/etc, so "language plpgsql".
tell we are using sql here.
- "as $" (it is a doulbe dollar actually) on third line and "$" at the last most line to avoid escape characters of any string error in between area.<br/>
- the procedure body, where all the logic is written is in between "begin" and "end;" keywords.
- we could have used "create procedure" only, but if we want to update an existing procedure we can use "create or replace procedure".

![33](https://user-images.githubusercontent.com/33677647/204255638-049790d3-092b-4270-aa34-7c6d0bf10b00.JPG)

as if we write any escape character, it will generate error :
 
 but when we put an "E" and "\" at the beginning of the escape character, they error will be resolved, but we will have to do this for each escape character which is a long process,
 
![1](https://user-images.githubusercontent.com/33677647/204255172-9fbe7a75-5a0c-4704-922d-76328c89f4aa.JPG)
![2](https://user-images.githubusercontent.com/33677647/204255240-ddda918c-7013-4318-b7a7-2775a910d158.JPG)

so the alternate solution is that we put a doulbe $ at the start and end, any escape character in between these dollar sign will not generate errors.

![3](https://user-images.githubusercontent.com/33677647/204255289-1a05cca2-8469-460d-8c6f-93b511551752.JPG)
