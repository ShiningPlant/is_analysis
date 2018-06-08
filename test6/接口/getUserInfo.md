### 接口：getUserInfo 

用例： 查看个人信息,修改个人信息

    功能： 查看用户的所有信息。

    权限： 学生/老师：查看自己的信息，必须先登录，不能查看其他用户的信息。

    API请求地址： 接口基本地址/v1/api/getUserInfo

    请求方式 ： GET

请求参数说明:
    
| 参数名称 | 说明 |
|:------:|------|
| user_id | 用户的ID号，对应表USERS.USER_ID的值 |

返回实例1：

    {         
      "status": true,
      "info": null,
      "student_id":"201510414208",    
      "name":"李星荟",
      "departmentt":"软件工程二班"
      "github_username":"ShiningPlant",
      "type":"学生"    
      "discipline_name":"信息系统分析与设计"        
    }
    


返回实例2：

    {         
          "status": true,
          "info": null,
          "teacher_id":"226548",    
          "name":"李某某",
          "github_username":"hihihi",
          "type":"老师",
          "department": "信息科学与工程学院"
     
     }
     
返回参数说明：

| 用例名称 | 修改密码 |
|:------:|------|
| 参数名称 | 说明 |
| status | bool类型，true表示正确的返回，false表示有错误|
| info	| 返回结果说明信息|
| student_id	| 学号|
| teacher_id	| 工号|
| name	| 用户的真实姓名|
| department| 班级或者部门名称|
| github_username	| gitHub用户名|
| type	| 用户类型：老师或者学生|
| discipline_name	| 选课名称|