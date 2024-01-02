
# Coffee Manager - Go, Chi, PostgreSQL
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

A sweet and simple CRUD API for coffee lovers like you and me.   


## Run Locally

Clone the project

```bash
  git clone https://github.com/abhinavthapa1998/coffee-manager.git
```
Start the server
```bash
  make run
```
Stop the server
```bash
  make stop 
```
Build the binary
```bash
  make build
```




## API Reference

#### Get All Coffees

```http
  GET /api/v1/coffees/coffee
```
#### Get Coffee By Id
```http
  POST /api/v1/coffees/coffee/{id}
```
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. id of the coffee |

#### Create Coffee
```http
  POST /api/v1/coffees/coffee
```
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. name of the coffee |
| `image` | `string` | **Required**. image of the coffee |
| `region` | `string` | **Required**. region of the coffee |
| `roast` | `string` | **Required**. roast of the coffee |
| `price` | `number` | **Required**. price of the coffee (in cents) |
| `grind_unit` | `string` | **Required**. grind_unit of the coffee |

#### Update Coffee By Id
```http
  PUT /api/v1/coffees/coffee/{id}
```
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Optional**. name of the coffee |
| `image` | `string` | **Optional**. image of the coffee |
| `region` | `string` | **Optional**. region of the coffee |
| `roast` | `string` | **Optional**. roast of the coffee |
| `price` | `number` | **Optional**. price of the coffee (in cents) |
| `grind_unit` | `string` | **Optional**. grind_unit of the coffee |

#### Update Coffee By Id
```http
  DELETE /api/v1/coffees/coffee/{id}
```
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `string` | **Required**. id of the coffee |
