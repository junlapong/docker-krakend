# Docker KrakenD

## Run

	./run.sh

## Test

	http :8080/api/users/1

	HTTP/1.1 200 OK
	Content-Length: 509
	Content-Type: application/json; charset=utf-8
	Date: Tue, 18 Jun 2019 05:25:42 GMT
	X-Krakend: Version 0.9.0
	X-Krakend-Completed: false

    {
        "address": {
            "city": "Gwenborough",
            "geo": {
                "lat": "-37.3159",
                "lng": "81.1496"
            },
            "street": "Kulas Light",
            "suite": "Apt. 556",
            "zipcode": "92998-3874"
        },
        "company": {
            "bs": "harness real-time e-markets",
            "catchPhrase": "Multi-layered client-server neural-net",
            "name": "Romaguera-Crona"
        },
        "email": "Sincere@april.biz",
        "id": 1,
        "name": "Leanne Graham",
        "phone": "1-770-736-8031 x56442",
        "username": "Bret",
        "website": "hildegard.org"
    }
