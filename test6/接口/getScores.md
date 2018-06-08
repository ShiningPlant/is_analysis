### 接口：getScores 

用例： 查看成绩

    功能： 返回一个学生的所有实验成绩和实验评价。

    权限： 根据课程编号及学号返回成绩列表
    
    API请求地址： 接口基本地址/v1/api/getScores

    请求方式 ： GET
    
请求实例：

    {
      "student_id": "201510414208"
          "discipline_id": "056482",
     }

请求参数说明:

| 参数名称 | 说明 |
|:------:|------|
| student_id |	学生的学号|
| discipline_id | 课程编号 |

返回实例：

    {         
      "status": true,
      "info": null,    
      "student_id": "201510414208", 
      "name": "李星荟", 
      "grade":90,       
      "data":[
             {
              "test_id":1,
              "web": true, 
              "grade": 93, 
               "item_title":"用例图及规约：10、……"
               "comment":"类图和接口设计一致",
               "update_date": "2018-04-02 18:25:11"
               "grades_percent":"20%"
               }, 
               {               
                ...其他实验
               }
               ] 
     }
     
返回参数说明：

| 参数名称 | 说明 |
|:------:|------|
| status |	bool类型，true表示正确的返回，false表示有错误|
| info |	返回结果说明信息|
| student_id |	学号|
| name |	真实姓名|
| item_title  |	每个实验的具体评分项|
| grades_percent |	每个实验占总成绩的百分比|
| test_id |	实验编号|
| web |	本实验的GitHub网页是否存在|
| grade |	本实验总成绩 |
| comment |	本实验老师的评价|
| update_date |	本实验老师的批改日期|