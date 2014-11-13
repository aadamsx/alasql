# To do
## URGENT

* SELECT 1+1
* FOREIGN KEY
* CREATE INDEX
* DROP INDEX
* DROP CONSTRAINT
* ALTER TABLE ADD COLUMN
* ALTER TABLE DROP COLUMN

* Add check for CROSS JOIN (that there is no USING or ON clause)
* Change INNER to CROSS
* NATURAL JOIN (if needed)

* console
* table.pk.pkrightfns, table.pk.pkrightfn, hh
* table.fks[].fkleftfns, table.fks[].fkleftfn, table.fks[].tableid, fks[].fkrightfns, table.fks[].fkrightfn
* INSERT, DELETE, UPDATE with primary and foreign keys

* CREATE TRIGGER  and triggers
* JOIN (subquery)
* Group by formula
* WITH clause
* documentation
* SELECT FROM nevenending stream (for Node.js), including INNER, LEFT, SEMI JOIN
* CURSORS
* Sandbox for SQL - like SQLFiddle, alasqlfiddle.
* db.indexAll(table)
* Precompiled insert for tables: 
* "SELECT aaa.* FROM :aaa" without AS clause
* compile flags for query (arrayofobjects, value, array, arrayofarrays)
* Aggregation formula GROUPFN()

## FEATURES TO BE IMPLEMENTED SOON
## MOBILE APPLICATIONS SUPPORT

* WinJS
* Apache Cordova
* PhoneGap

## BUSINESS INTELLIGENCE

* d3
* OLAP

## FRAMEWORKS

* jQuery
* AngularJS

## JAVASCRIPT

* WebWorker

## Applications

* Command-line utility for text files

* BEGIN COMMIT ROLLBACK
* INSERT INTO test SELECT 'a' UNION ALL SELECT '10'
* AVG aggregator (http://www.w3schools.com/sql/sql_func_avg.asp)
* SELECT INTO table IN database FROM query [like this](http://www.w3schools.com/sql/sql_select_into.asp)
* Change grammar for LogicValues
* GO* Separate branch on github.com for development

Optimization

* WHERE multiple optimization
* Performance Tests based on SQLite [tests](http://www.sqlite.org/speed.html)
* Pass [SQL Logic Test](http://www.sqlite.org/sqllogictest/doc/trunk/about.wiki)
* Optimization for EXISTS subqueries (check if column is from outer select)
* Replace join recursion with loop (may be faster) [like here](http://architects.dzone.com/articles/sql-execution-plans-javascript)
* Optimizations for joins and subqueries
* SELECT * FROM f JOIN g ON f1 = g2 AND F1(f) = G1(g) AND F2(not g) = G2(not f) 
* FOREIGN KEY JOINS
* WHERE a OR b optimization
* ORDER BY WITH index
* Optimization of WHERE and JOINS with indices 
* Indices with hash
* Dirty data and indices update
* Code refactoring
* Performance tests and optimization
* Minimize size
* Indices with insert/delete/update procedure
* EXPLAIN QUERY PLAN (like [SQLite does](https://www.sqlite.org/eqp.html))
* Combine selectwhere and groupfn functions
* Semi-joins (for outer joins) 
* Expand outer join to N tables (not only two)
* INSERT INTO SELECT statement

SELECT AND OTHER SQL STATEMENTS

* Fast join of single value with indices (PRIMARY KEY)
* GROUP BY ALL
* FULL OUTER JOIN
* ANTI-JOINS, SEMI-JOINS
* [NATURAL JOIN](http://docs.oracle.com/javadb/10.6.2.1/ref/rrefsqljnaturaljoin.html#rrefsqljnaturaljoin)
* Constrains, Foreign Keys, Primary key, cascade delete and update
* Types, NULL, NOT NULL
* Database.schema.table.field
* Constrains
* Keys
* Null not null
* Primary key
* Rowversion, rowversion on insert, delete
* JavaScript functions
* Identity 1,1, unique fields
* SELECT TOP
* FETCH 
* Case operator
* Views (?)
* Cursors
* SQLite compatibility: functions
* SQL-standards - check [this](https://www.sequelsphere.com/dbdocs/supported-sql/)
* SQL-functions - check [this](https://www.sequelsphere.com/docs/latest/doc/Supported%20SQL%20Functions.html)

BUGS

* Tableid and fields to lowercase
* Aggregators without groups
* 'SELECT wrongfield FROM table' gives something wrong 
* Change order of groupfn() and selectfn(), and check havingfn vs selectfn

PERSISTENCE

* WebSQL
* localStorage / sessionStorage
* IndexedDB
* lawnchair.js
* Serer synchronization JavaScript plugin (like [WebSqlSync](https://github.com/orbitaloop/WebSqlSync))

DEVELOPMENT

* Minifiication

REALIZATION

* WebWorkers
* Redis, levelDB, IndexDB, localStorage for persistence 
* Persistence
* Split parsing, compilation, and execution functions
* JSon sql definition
* Compile to asm.js
* Executor
* Compiled procedures
* Compiled statements
* alasql2js compiler
* Better parser and SQL-formatter

ANYDATABASE

* Any database
* Node.js server
* Pass-thru database

COMPATIBILITY

* Compatibility
* Realize SQLite functions (from [documentation](http://kripken.github.io/sql.js/documentation/))
* Test with ie and Firefox browsers
* Tests for different browsers (IE!!!)
* Crossfilter, lodash and underscore speed comparision
* Cover WebSQL and Sql.js with own functions (for simple migrating)
* Be compatible with [w3school](http://www.w3schools.com/sql/default.asp)
* [Oracle syntax](http://docs.oracle.com/javadb/10.6.2.1/ref/rrefclauses.html)
* Check [SQL BNF](http://www.contrib.andrew.cmu.edu/~shadow/sql/sql2bnf.aug92.txt)

OTHER NEEDED FUNCTIONALITY (MORE THAN SQL)

* OLAP
* Pivot operator
* Totals (this is non-SQL functionality, but required)
* Running totals 
* Hierarchy totals
* Totals with insert/delete/update procedure

MDX
* MDX parser
* MDX processor

SAMPLES

* Check for compatibility with [W3C SQL demo database](http://www.w3schools.com/w3Database.js)
* Console [like](http://www.moxleystratton.com/files/sqittle.html) 
* One more [sample](http://yradtsevich.github.io/pure-js-websql/test/index.html)
* Create tutorial database on https://github.com/txje/js-sql-tutorial for best console

### Version 0.2 - NoSQL supports

* JavaScript search like MongoDB

### Version 0.3 - OLAP + MDX

* Mini MDX parser
* JavaScript in-memory OLAP functionality (additional library)


OTHER

* Create site alasql.org
* Review [textql project](https://github.com/dinedal/textql), [q](https://github.com/harelba/q), 
* [presto](http://prestodb.io/), [h2](http://www.h2database.com/html/grammar.html)