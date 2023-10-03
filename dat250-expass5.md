# Report Expass 5
Link to GitHub: https://github.com/EndreSletnes/dat250-expass5

## Tasks
* Task 1
  Everything worked fine.
* Task 2
  Modified the files to work as in the tutorial and built the jar file with gradle. I could then run the jar with the command "java -jar build/libs/expass5-0.0.1-SNAPSHOT.jar"
* Task 3
  Changed the mapping from "/" to "/hello" in HelloController so that the mapping didn't overwrite the index.html.
* Task 4
  Removed the commandlinerunner from task 2 and replaced it with the one for task 4.  

## Techical problems
* IntelliJ didn't recognize the gradle build because it was set to default version 21, so I had to change it to 17.
* In task 2 when using curl to access localhost:8080 I had to use http:// first.
* In task 4 I didn't add the dependency to h2database so on runtime I got an error.
