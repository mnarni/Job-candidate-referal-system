## Project Setup
1. IDE: IntelliJ IDEA (v2022.3.3 or later)
1. Java Version: 17
1. Gradle Version: >= 7.3
1. ###### Set Gradle location in the IDE (for running the app in the IDE)
   > IntelliJ (macOS)
      - Intellij IDEA `>` Settings… `>` Build, Execution, Deployment `>` Build Tools `>` Gradle
      - Select the project under __`Gradle Projects`__.
      - Make the following change:
        - _Use Gradle from:_ `Specified location` : __&lt;gradle home&gt;__, e.g. `$HOME/.sdkman/candidates/gradle/current/bin`
        <br>** `$ whereis gradle` _can show the path to gradle_.
      - Click `Apply`.
      - Click `OK`.
1. Build the project from the terminal:
   > `$ gradle build` <_RETURN_>
1. Run the program from the terminal:
   > `$ gradle bootRun` <_RETURN_>
   > 
## Access the [in-memory] database
1. [project root] `$ gradle bootRun` <_RETURN_>
1. [Browser] http://localhost:8008/h2-console
    - `Saved Settings: ` Generic H2 (Embedded)
    - `Setting Name: ` Generic H2 (Embedded)
    - `Driver Class: ` org.h2.Driver
    - `JDBC URL: ` jdbc:h2:mem:jcrs
    - `User Name: ` sa
    - `Passwword: ` <_BLANK_>
    - <button>Test Connection</button>
    - <button>Connect</button>


## Docker
- Install Docker: [macOS](https://formulae.brew.sh/formula/docker), [Windows](https://docs.docker.com/desktop/install/windows-install/)
- [project root] `$ chmod a+x scripts/*.sh` <_RETURN_>
- Run program: `$ scripts/start.sh` <_RETURN_>
- Stop program: `$ scripts/stop.sh` <_RETURN_>


