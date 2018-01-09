# 采集器相关

## 获取前置采集节点列表
1.requst `GET /api/agents`  
2.response   

   * **成功**
    
   http status : `200`
    
   Content-Type : `application/json`
   
   body:
```
[
  {
    "configuration": {
      "agentId": "string",
      "strategies": [
        {
          "rules": [
            {
              "expression": "string",
              "id": "string",
              "priority": 0
            }
          ]
        }
      ]
    },
    "host": "string",
    "id": "string",
    "name": "string",
    "port": 0,
    "status": "Offline",
    "version": "string"
  }
]
```

## 注册前置采集节点
1.requst `POST /api/agents`  

  consumer: `application/json`
  
  body: 
```json
[
  {
    "configuration": {
      "agentId": "string",
      "strategies": [
        {
          "rules": [
            {
              "expression": "string",
              "id": "string",
              "priority": 0
            }
          ]
        }
      ]
    },
    "host": "string",
    "id": "string",
    "name": "string",
    "port": 0,
    "status": "Offline",
    "version": "string"
  }
]
```

2.response   

   * **成功**
    
   http status : `200`
    
   Content-Type : `application/json`
   
   body:
```
[
  {
    "configuration": {
      "agentId": "string",
      "strategies": [
        {
          "rules": [
            {
              "expression": "string",
              "id": "string",
              "priority": 0
            }
          ]
        }
      ]
    },
    "host": "string",
    "id": "string",
    "name": "string",
    "port": 0,
    "status": "Offline",
    "version": "string"
  }
]
```

## 更新前置采集节点
1.requst `POST /api/agents/{id}`  根据根据url的id及body中的Agent对象更新前置节点

  consumer: `application/json`
  
  body: 
```json
{
  "configuration": {
    "agentId": "string",
    "strategies": [
      {
        "rules": [
          {
            "expression": "string",
            "id": "string",
            "priority": 0
          }
        ]
      }
    ]
  },
  "host": "string",
  "id": "string",
  "name": "string",
  "port": 0,
  "status": "Offline",
  "version": "string"
}
```

2.response   

   * **成功**
    
   http status : `200`
    
   Content-Type : `application/json`
   
   body:
```
{
  "configuration": {
    "agentId": "string",
    "strategies": [
      {
        "rules": [
          {
            "expression": "string",
            "id": "string",
            "priority": 0
          }
        ]
      }
    ]
  },
  "host": "string",
  "id": "string",
  "name": "string",
  "port": 0,
  "status": "Offline",
  "version": "string"
}
```

## 启动前置采集节点
1.requst `POST /api/agents/{id}/?operation=start`  根据根据url的id启动前置采集节点

2.response   

   * **成功**
    
   http status : `200`

## 停止前置采集节点
1.requst `POST /api/agents/{id}/?operation=stop`  根据根据url的id启动前置采集节点

2.response   

   * **成功**
    
   http status : `200`

## 删除前置采集节点
1.requst `DELETE /api/{id}`  根据根据url的id启动前置采集节点

2.response   

   * **成功**
    
   http status : `200`
    
