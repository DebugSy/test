# 汇总查询
## 获取单条明细记录
1.requst `GET /api/record/{table}/{id}`  根据根据url中的表及id获取记录

2.response   

   * **成功**
    
   http status : `200`
   
## 获取分页记录  
1.requst `GET /api/record/{table}/page`  根据根据url中的表名及参数中分页信息获取记录 

2.response   

   * **成功**
    
   http status : `200`
 
## 获取聚集结果
1.requst `GET /api/record/{table}/aggregation`  根据根据url中的表名及参数中获取聚集结果

2.response   

   * **成功**
    
   http status : `200`
   ```
