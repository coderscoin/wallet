# wallet

## Peer network reference

### Get the balance of a user
```https
METHOD getBalance
```
This returns the balance of user
#### Request
| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `type` | `string` | **Required**. Method name |
| `data` | `string` | **Required**. Username of user |
#### Example Response
```json
{"type":"dataResponse","data":3454}
```

### Submit a transaction to the network
```https
METHOD newTransaction (soon)
```
This returns the balance of user
#### Request
| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `type` | `string` | **Required**. Method name |
| `data` | `string` | **Required**. Username of user |
#### Example Response
```json
{"type":"dataResponse","data":3454}
```

