## Difference between SetupSuite & SetupTest in Testify Suites 
[Stackoverflow](https://stackoverflow.com/questions/50200933/difference-between-setupsuite-setuptest-in-testify-suites)

`SetupTest`: It is used so that each individual test function runs with a clean environment.
`SetupSuite`: SetupSuite is useful in cases where the setup code is time consuming and isn't modified in any of the tests. An example of when this could be useful is if you were testing code that reads from a database, and all the tests used the same data and only ran SELECT statements. In this scenario, SetupSuite could be used once to load the database with data.