# Back End Test Project CODEROCKR

## libraries used
### Lumen
just Lumen, which is a micro php framework derived from Laravel.
I really like the structure of Laravel and its well done documentation. Since the framework has a lot of ready-made stuff that speeds up the work, such as the connection to the database, and the ORM, as well as configurations for tests.
## how to build
to terminal run the command below
```bash
  docker-compose up -d
```
with the containers running, access the php container and install the composer dependencies

```bash
  docker exec -it investment_portfolio_app bash
```
```bash
  composer install
```
if you need, permission in the log directory that is inside the storage

```bash
  chmod -R 777 storage/log
```
## api documentation
the server will run on `http://localhost:8000` 

### endpoints

---
## Investor
### GET ALL INVESTORS
#### Example URI
`GET http://localhost:8000/api/v1/investor`
#### URI Paramenters
#### Headers 
`Content-Type: application/json`
#### Request
#### Response
```json
{
    "message": "success",
    "error": false,
    "data": [
        {
	    "id": "9d352490-7938-46b1-aca4-6d71f527903f",
	    "name": "paulo henrique",
	    "created_at": "2022-02-20T21:55:56.000000Z",
	    "updated_at": "2022-02-20T21:55:56.000000Z"
	}
    ]
}
```

---

