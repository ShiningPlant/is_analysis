### 接口：getStudentList

用例： 学生列表

    功能： 根据课程编号显示本课程所有学生列表。

    权限： 学生/老师

    API请求地址： 接口基本地址/v1/api/getStudentList

    请求方式 ： GET
    
请求实例:

     {
      "discipline_id": "025373"
     }

请求参数说明: 

| 参数名称 | 说明 |
|:------:|:------:|
| discipline_id | 课程编号 |

返回实例：

    { 
         "status": true,
         "info": null,
         "data": {
             "students": [{
                 "student_id": "201510414208",
                 "class": 软件工程二班,
                 "web": Y,
                 "user": {
                     "user_id": "201510414208",
                     "name": "李星荟",
                     "github_username": "ShiningPlant",
                 }
             },{
                 ...
             }]   
         }    
     }
    
返回参数说明：

| 参数名称 | 说明 |
|:------:|------|
| status | bool类型，true表示正确的返回，false表示有错误|
| info |	返回结果说明信息|
| WEB |	网址是否正确|
| GITHUB_USERNAME |	github用户名|
| STUDENT_ID |	学号|
| CLASS	| 班级|
| NAME | 用户真实姓名|