# Project Rapport - DAT250: expass1
- DockerHub repository: https://hub.docker.com/r/esletnes/dat250

## Tasks
- I found WSL hard to work with, so I installed everything needed on Windows instead.
- Step 1: I made a new repository on GitHub and used IntelliJ to clone it.
- Step 2: I used "gradle init" to initialize the project.
- Step 3: I added dependencies and made the app run. I got rid of the "Javalin: It looks like you don't have a logger in your project." warning by adding a dependency to slf4j-simple in the build.gradle.kts file.
- Step 4: I added a test I knew was failing and got an error message that one test failed when running "./gradlew.bat check".
- Step 5: I used docker and when running "docker images" I got the image I just created and no others. Using the built-in docker features of IntelliJ I pushed the image to DockerHub.


## Validation
- I used the command "./gradlew.bat check" to check that the conversion worked.
- I ran the app and checked that it worked in the browser.
- I ran the docker image after pushing to DockerHub, and it ran fine, although I could not check it in the browser as mentioned in "Technical problems".


## Technical Problems
- I tried using the built-in Gradle functionality in IntelliJ, but it didn't work. Instead, I used the terminal.
- Using gradle init I got an error saying "'no.hvl.dat250.798192.exp1' is not valid source package name". I solved this by using "dat250assignment1" as source package name instead.
- When running a docker container with my image from DockerHub I can't access localhost/9000, and no ports are exposed. I have not solved this issue.