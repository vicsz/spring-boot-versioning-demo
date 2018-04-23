
__Simple DEMO of adding GIT SCM information and BUILD information to the actuator info endpoint to easily identify deployed versions!!__ 

Highly recommend for all project to be able to precisely tell the exact version of code deployed to an environment as well as build information.

__Hit the actuator /actuator/info endpoint at:__

#curl localhost:8080/actuator/info

You should see something simliar to the following ( note that the git properties will only show if the directory is part of a valid GIT repository)

```json
{
	"git":{
		"commit":{
			"time":"2018-04-20T18:11:28Z",
			"id":"f704f36"
		},
	"	branch":"master"
	},
	"build":{
		"version":"1.0.0.2",
		"artifact":"demo",
		"name":"demo",
		"group":"com.example",
		"time":"2018-04-23T13:11:00.556Z"
	}
}
```

__ Maven Notes  __

Maven instructions are available at :

__https://docs.spring.io/spring-boot/docs/current/reference/html/howto-build.html#howto-build-info__

__86.1 Generate Build Information__

__86.2 Generate Git Information__