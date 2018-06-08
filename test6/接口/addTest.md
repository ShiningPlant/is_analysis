### 接口：addTest

用例：新增实验 

    功能： 创建指定课程的实验信息。

    权限： 老师

    API请求地址： 接口基本地址/v1/api/addTest

    请求方式 ： POST

请求实例：

    {
      "disciplines_id": "05411",
      "tests_id": 1,
      "tests_title": "软件设计",
      "tests_content": "熟练掌握类图的画法",
    }  
    
请求参数说明:

| 参数名称 | 说明 |
|:------:|------|
| disciplines_id |	课程编号|
| tests_id |	实验编号|
| tests_name |	实验名称|
| tests_content |	实验内容|


返回实例：

    {         
      "status": true,
      "info": null,    
    }
    
返回参数说明：

| 参数名称 | 说明 |
|:------:|------|
| status |	bool类型，true表示正确的返回，false表示有错误|
| info |	返回结果说明信息|