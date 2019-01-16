# my-todo-everyday

###### แก้ไขครั้งล่าสุด 16/01/2019 เวลา 16:27

### `POST` /task/add

#### Request body
| Attribute Name | Attribute Type  |  Attribute Value  | Description |
| ------------- | ------------- | ------------- | ------------- |
| head | `string` | ฝึก Hapi | หัวข้อของงานที่ทำ |
| description | `string` | แบ่งทีมทำ Hapi Task to do | คำอธิบายเนื้องาน |
| type | `string` | Train | ประเภทของงานที่ทำ |
| time | `string` | 04:15 | จำนวนเวลาในการทำงาน

#### ตัวอย่าง Request body
```json
{
  "head": "ฝึก Hapi",
  "description": "แบ่งทีมทำ Hapi Task to do",
  "type": "Train",
  "time": "04:15"
}
```

#### Response


| Attribute Name | Attribute Type  |  Attribute Value  | Description |
| ------------- | ------------- | ------------- | ------------- |
| status | `string` | 200,500 |  |
| message | `string` | success,failed |   |

##### Response Code `200`
```json
{
    "status": 200,
    "message": "success"
}
```

##### Response Code `500`
```json
{
    "status": 500,
    "message": "failed"
}
```
