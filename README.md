#  packages the database structure in JSON

## Build jar
Execute `./mvnw -Dmaven.test.skip=true install` command in repository root folder

## Run
Execute `java -jar db-parser-0.0.1.jar --spring.datasource.url=<url> --spring.datasource.username=<username> --spring.datasource.password=<password>` command near the `.jar` file
<br /><br />where you should change `<url>`, `<username>`, `<password>` values to your params ***without triangular bracket***
<br /><br />my example: `java -jar db-parser-0.0.1.jar --spring.datasource.url=jdbc:postgresql://localhost:5432/test --spring.datasource.username=achek --spring.datasource.password=impsstabb`

## Result
`<database name>_structure.json` file will be generated near the `.jar` file
