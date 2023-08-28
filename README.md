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
| `transaction` | **Required**. Transaction object with TSK |
| `data` | `string` | **Required**. Data of apps |
#### Example Request
```json
{
        	"type": "newTransaction",
	        "transaction": {
	            "from": "johndoe",
	            "to": "petertill",
	            "amount": 2,
	            "tsk": "hfdsuhiufhszgwez43423iigvsizibsvdbisfd&@yxcxcrffds"
	        },
	        data: [{"product": 3421}]
    	}
```
#### Example Response
```json
{"type":"dataResponse","data":3454}
```

