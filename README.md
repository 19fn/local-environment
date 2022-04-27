# Local Environment

## Getting Started

### Prerequisites
- `Java` should be installed (v8.0 or more recent is fine but we prefer 11.0 and newer)
- `Maven` should be installed (recommended v3.8.5 or higher)
- `Docker` should be installed (recommended v20.10.14 or higher)
- `Docker Compose` should be installed (recommended v1.29.2 or higher)

## Using Local Environment

### Change Project Name
You can change the path to your target directory as you wish. Also, you should change the project name in the docker-compose.yml file to your actual project.
```sh
volumes:
         - "path/to/target/:/opt/target/"

.
.
.

command: ["java","-jar","/opt/target/your-actual-project.jar"]
```

### Control.sh Script
It's a good idea to inspect the control script. You can look through it so everything looks normal, then running it:
```sh
[!] Usage: ./control.sh [start] || [stop]


	Command:	Description:
	start		Start local environment container
	stop		Shutdown local environment container
```
