# SQL_Stored-Procedure

Stored procedures are used to do the work that simple sql query can not do.
- It starts with the keyword "create or replace prcedure than_here_name_of_your_procedure (nameOfFirstParameter ItsDataType, nameOfSencondParameter ItsDataType)"
- then on second line, specificly in postgreSQL you have to specify that which language we will use here,<br/> because postgreSQL also supports python/c++/etc, so "language plpgsql".
tell we are using sql here.
- "as $" (it is a doulbe dollar actually) on third line and "$" at the last most line to avoid escape characters of any string error in between area.<br/>
- the procedure body, where all the logic is written is in between "begin" and "end;" keywords.
