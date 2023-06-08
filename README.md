# my-first-repository
	Найти информацию о всех контрактах, связанных с сотрудниками департамента «Logistic». Вывести: contract_id, employee_name

   SELECT executor.contract_id, employees.name FROM employees
  JOIN executor ON employees.id = executor.tab_no
	 WHERE employees.department_id=(SELECT id FROM Department WHERE Name='Logistic')  
