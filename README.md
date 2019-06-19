# Docker KrakenD

## Docker

### Run

	docker run -p 8080:8080 -v $PWD/config:/etc/krakend/:ro devopsfaith/krakend

### Test

	http :8080/api/users/1

	HTTP/1.1 200 OK
	Content-Length: 509
	Content-Type: application/json; charset=utf-8
	Date: Tue, 18 Jun 2019 05:25:42 GMT
	X-Krakend: Version 0.9.0
	X-Krakend-Completed: false

    {
		...
	}

## macOS

### Install

	brew install krakend

### Run

	krakend -c config/krakend-short.json run

### Test

	http :8080/api/todos/1

	HTTP/1.1 200 OK
	Access-Control-Allow-Credentials: true
	Cache-Control: public, max-age=14400
	Content-Length: 99
	Content-Type: application/json; charset=utf-8
	Date: Wed, 19 Jun 2019 02:00:36 GMT
	Etag: W/"63-+s0zIP5ZEQN9hypVJUneLybJ+L0"
	Expires: Wed, 19 Jun 2019 06:00:36 GMT
	Pragma: no-cache
	X-Content-Type-Options: nosniff
	X-Krakend: Version 0.9.0
	X-Krakend-Completed: false
	X-Powered-By: Express

	{
		...
	}
