## Oracle-SQL


### Database Concepts

1. What is an Entity?: The smallest unit contained meaningful set of data is called entity. Rows Cols or even tables are entities.
2. What is the relationship?: логическа връзка между две или повече ентитита или по скоро таблици ако вземе ентититата като таблици.
    Чрез съхраняването на ID във всеки запис на таблизата просто създаваме връзка. 

    В Оракъл може да имаме доста плъгъбл бази данни с един корен (Container Database) след 12c версията. Елиминира възможноста да правим много бази които не са големи и изискват сървър. На един за да олесни работата на DBA и оскъпяването на сървърите.

 Оракъл базите имат много дб обекти категоризирани в 2 субекта: Schema objects и Nonschema objects. 
 Schema objects са тези които се създават от потребителя и са във връзка със схемата на базата. 
 Nonschema objects са тези които се създават от системата и са във връзка със сървъра.

 # Table:
  Основна единица на базите данни за съхранение на данни. Състои се от редове и колони.
 # View:
  Виртуална таблиза която се създава от една или повече таблици за да провидне достъп до събсет от колони или редове.
  Изгледа е просто SQL скрипт с име като таблицата и когато се направи заявка към него той се изпълнява и връща резултат.
    Изгледа се използва за да се скрият данни от потребителите.

# Constraint:
    Ограничение на данните в таблизата. Може да бъде на колона или на цялата таблиза. 
    Ограниченията се използват за да се гарантира че данните в таблизата са валидни. 
    Например: NOT NULL, UNIQUE, PRIMARY KEY, FOREIGN KEY, CHECK, DEFAULT
  
# Index: 
    Структура която се създава върху една или повече колони на таблизата за да се ускори търсенето на данни.
    Индексите се използват за да се намали времето за търсене на данни в таблизата. 
    Индексите се създават от един или повече полета на таблизата и се съхраняват в отделна структура. 
    
# Sequence:
    Обект който се използва за да се генерира поредица от уникални числа. 
    Поредицата може да бъде възходяща или низходяща. 
    Поредицата се използва за да се генерира уникално число за всяка нова запис в таблизата. 

# Synonym:
    Обект който се използва за да се създаде алтернативно име на друг обект. 
    Синонимите се използват за да се скрият имената на обектите от потребителите. 
    Пример: SELECT * FROM employees; SELECT * FROM emp; SELECT * FROM emp_view; SELECT * FROM emp_synonym;

# Materialized View

# Functions and Procedures
    Функциите връщат стойност, а процедурите не връщат стойност.
# Triggers
    Тригерите са обекти които се изпълняват автоматично при определено събитие. 
    Събитието може да бъде INSERT, UPDATE, DELETE или DDL събитие. 
    Тригерите се използват за да се изпълни допълнителна логика при определено събитие. 
    Например: да се запише в друга таблиза при всяко ново записване в таблизата.

# Packages
    Пакетите са обекти които съдържат процедури и функции. 
    Пакетите се използват за да се групират процедурите и функциите в един обект. 
    Пакетите се използват за да се организират процедурите и функциите в базата данни. 
    
# Database Links
    Връзката между 2 физически дб сървъра.

# Non-schema objects
    Тези обекти се създават от системата и са във връзка със сървъра. 


 ## What is Schema? 
    Колекция от обекти за всеки потребител в Oracle Database.


    Пример:
        HR - Human Resources
        Схемата може да има:
        Tables, Views, Indexes, Sequences, Synonyms, Materialized Views, Functions, Procedures, Triggers, Packages, Database Links, Non-schema objects

## What is SQL?
    SQL е език за структурирана заявка. Език за интеракция с бази данни. Използва се в Data Science, Database Administration, Web Development, etc.
    Лесен ли е? Да, лесен е за изучаване и използване. но може и да е комплексен за някои заявки.



