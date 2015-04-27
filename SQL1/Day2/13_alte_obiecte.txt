-- alte obiecte

create view dep2_test as
select department_id, department_name
from departments;

drop view dep2_test;

CREATE SEQUENCE test_SQ
  START WITH 1
  MAXVALUE 999999999999999999999999999
  MINVALUE 1
  NOCYCLE
  NOCACHE
  NOORDER;
  
select test_SQ.NEXTVAL
        from dual;   
  
select test_SQ.CURRVAL
        from dual;
        
ALTER SEQUENCE test_SQ
  MAXVALUE 999999999
  MINVALUE 1
  NOCYCLE
  NOCACHE
  NOORDER; 
  
create index epm_idx on emp_TEST (dep_id);  

create synonym emp for employees;

select *
        from emp;
        
drop synonym emp;