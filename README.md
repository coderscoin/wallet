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
### Submit mined block

```https
  POST /mine/
```
#### Request
| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `latesthash` | `string` | **Required**. The computed hash of the latest block |
| `proof` | `string` | **Required**. The proof returned from the PoW algorithm |
| `newblock` | `list` | **Required**. The newly mined block's details |
| `miner` | `string` | **Required**. The username of the miner |

#### Response
| Code | Description                       |
| :-------- | :-------------------------------- |
| `200` | The mining is successful and has been accepted by the network. |
| `403` | The user was banned from the platform due to fraud detected or the last block was not validated |
| `500` | Mining failed, the network rejected the request because it is incorrect. |
