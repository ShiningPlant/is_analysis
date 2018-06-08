### 接口：selectDisciplineByTeacher
       
用例： 学生选课
       
           功能： 学生进行选择课程。
       
           权限： 学生
       
           API请求地址： http://202.115.82.8:1522/v1/api/selectDisciplineByTeacher
       
           请求方式 ： GET
       
 请求实例：
       
           {
             "teacher_id": "2351"
             "term_id":"2018-1"
            }
            
请求参数说明:
       
       | 参数名称 | 说明 |
       |:------:|------|
       | teacher_id |	老师的工号|
       | type |	用户类型，老师|
       | term_id |	学期编号|
       
返回实例:

           {
             "status": true,
             "discipline_id":"1",
             "discipline_name":"软件系统分析与设计",
             "discipline_time":"周一上午1、2节课"
             "discipline_place":"10517"
             "discipline_population":"60"
             "discipline_hour":"48"
           }
         
返回参数说明：
       
       | 参数名称 | 说明 |
       |:------:|------|
       | status |	bool类型，true表示正确的返回，false表示有错误 |
       | discipline_id |	课程编号 |
       | discipline_name |	课程名称 |
       | discipline_time |	课程时间 |
       | discipline_place | 课程地点 |
       | discipline_poplution | 课程人数 |
       | discipline_hour |	课时 |
