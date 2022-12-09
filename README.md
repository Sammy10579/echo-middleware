# Build echo middleware

Example project of test assessment from imaginary company. Full text of the task can be found [here](docs/testtask.pdf)


### Build a middleware using echo framework

First of all, you should create a handler which sends how many days left until 1 Jan 2025 and response with HTTP 200 OK status code.

Secondly, build a middleware, which checks HTTP header `User-Role` presents and contains `admin` and prints `red button user detected` to the console (using default log package or any 3rd party) if so.

## Run

```shell
go run github.com/spatecon/echo-middleware-assessment/cmd/umbrella-test-task
```

## Test

```shell
curl --location --request GET '127.0.0.1:8080/status' \
--header 'User-Role: admin'
```


