
__Simple DEMO of adding GIT SCM information and BUILD information to the actuator info endpoint to easily identify deployed versions!!__ 


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