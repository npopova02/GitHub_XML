# XML
XML
		https://github.com/npopova02/XML

 21. Создать внешний репозиторий c названием XML.
	зайти в GitHub и создать новый репозиторий-  Repositories-> New->XML(name)-Public-Add a README file->Create repository
 
 22. Клонировать репозиторий XML на локальный компьютер.
	$ git clone https://github.com/npopova02/XML.git

 23. Внутри локального XML создать файл “new.xml”.
	cd new.xml
	$ touch new.xml

 24. Добавить файл под гит.
	$ git status
	$ git add new.xml
	
 25. Закоммитить файл.
	$ git commit -m "Adding a new empty file"
 
 26. Отправить файл на внешний GitHub репозиторий.
	$ git push 
	
 27. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
	$ vim new.xml
	<Person>
		<Personal>
			<Name> Попова Надежда Анатольевна </Name> 
			<Age> 38 </Age>
			<Pets> 1 </Pets>
			<Salary> $500 </Salary>
		</Personal>
	</Person>	
	
	Esc- выходим из редактирования
	:wq->Enter - сохраняем изменения
	
 28. Отправить изменения на внешний репозиторий.
	$ git push
	
 29. Создать файл preferences.xml
	$ touch preferences.xml

 30. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
	$ vim preferences.xml
	<Person>
	  <Preferences>
          <Film> Достучаться до небес </Film>
          <Series> нет </Series>
          <Food> Борщ </Food>
          <Season> Лето </Season>
          <Country> Индия </Country>
	  </Preferences>
	</Person>
	
	Esc- выходим из редактирования
	:wq->Enter - сохраняем изменения
	
 31. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
 $ cat> skills.xml
	добавить данные
	<Person>
	  <Skills>
          <Skill1> Linux GitBash </Skill1>
          <Skill2> Mobile testing </Skill2>
          <Skill3> Dev Tools </Skill3>
          <Skill4> SQL </Skill4>
          <Skill5> Postman </Skill5>
	  </Skills>
	</Person>
	Cntr+C - сохранение

 32. Сделать коммит в одну строку.
	$ git . && git commit -m "Adding preference and skills information"

 33. Отправить сразу 2 файла на внешний репозиторий.
	$ git push
	
 34. На веб интерфейсе создать файл bug_report.xml.
	зайти в репозиторий XML-> кнопка Add file-> ввести bug_report.xml в поле для названия файла
	
 35. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
	ввести текст коммита в поле для названия коммита-> нажать кнопку Commit new file 
 
 36. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
	открыть файл-> выбрать Edit this file(карандашик)-> добавить баг репорт в формате JSON
	
	<bug_report>
		<id> 1 </id>
		<summary> No login with valid username/password </summary> 
		<severity> Blocker </severity>
		<priority> High </priority>
		<status> Open </status>
		<precondition>  Valid data: Username- standard_user, password-secret_sauce </precondition>
		<steps_to_reproduce>
			<1> Go to www.saucedemo.com </1>
			<2> Enter valid Username/password combination </2>
			<3> Click [LOGIN] button </3>  
		</steps_to_reproduce>
		<actual_result> Login is not sucssesfull. Error message "Epic sadface: Username and password do not match any user in this service" appears </actual_result>
		<expected_result> Login is sucssesfull. The home page of the site appears </expected_result>
	</bug_report>
	
 37. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
	ввести текст коммита в поле Commit changes-> нажать кнопку Commit changes
	
 38. Синхронизировать внешний и локальный репозиторий XML
	$ git pull