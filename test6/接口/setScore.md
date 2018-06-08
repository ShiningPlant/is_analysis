### 接口：setScore 返回

用例： 评定成绩

    功能： 评定（修改）学生的成绩和评价。

    权限： 老师。

    API请求地址： 接口基本地址/v1/api/setScore

    请求方式 ： POST

请求实例：

    {
      "discipline_id": "00562"
      "student_id": "201510414208"
      "tests_grades": [{
                "tests_id": 1
                "grade": 90,
                 "comment": "实验要求基本完成，结构清晰简洁"
                 "update_date": "2018-05-29 11:46:27"
                "tests_grades": [{
                    "item_id": 1,
                    "rusult": 100,
                },{
                    "item_id": 2,
                    "result": 80,
                }]
            }]
    }    
    
请求参数说明:

| 用例名称 | 修改密码 |
|:------:|------|
| discipline_id	| 课程编号|
| student_id |	学号|
| tests_id	| 实验编号|
| result | 实验成绩|
| comment |	课程评价|
| update_date |	课程成绩批改时间|
| tests_grades | 实验成绩集合|
| grade| 某个实验成绩|
| comment | 某个实验评价|
| update_date | 某个实验批改时间|
| test_grades | 评分项成绩集合|
| item_id	| 评分项编号|
| result| 评分项成绩|

返回实例：

    {         
      "status": true,
      "info": null,    

    }
  
返回参数说明：

| 用例名称 | 修改密码 |
|:------:|------|
| 参数名称 | 说明 |
| status | bool类型，true表示正确的返回，false表示有错误|
| info	| 返回结果说明信息|