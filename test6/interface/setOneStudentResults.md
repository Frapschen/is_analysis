<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setOneStudentResults  [返回](../README.md)
用例： [评定成绩](../usecaseprinciple/evaluate_grades.md)

- 功能：
    设置一个学生的部分实验成绩和评语。
    
    输入参数result不为空，自动设置update_date为当前日期，表示同时设置批改日期。
    
    输入参数result为空，自动设置update_date为空，表示未批改。
    
- 权限：
    老师：可以查看所有学生的成绩。
    
- API请求地址： 
    接口基本地址/v1/api/setOneStudentResults

- 请求方式 ：
    POST
 
- 请求实例：  

        { 
            "student_id": "201510315203", 
            "test_id": 1,
            "course_id"
            "program1": 10,
            "rate1": 20,
            "comment1": "评价",
            "program2": 10,
            "rate2": 20,
            "comment2": "评价",
            "program3": 10,
            "rate3": 20,
            "comment3": "评价",
            "program4": 10,
            "rate4": 20,
            "comment4": "评价",
            "program5": 10,
            "rate5": 20,
            "comment5": "评价",
            "result": 91,
            "update_date": "2018-04-02 13:48:01"
        }

- 请求参数说明:       
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |student_id|学号|
   |test_id|实验编号|
   |course_id|实验编号|
  |program1|得分1|
  |rate1|占比1|
  |comment1|评价1|  
  |program2|得分2|
  |rate2|占比2|
  |comment2|评价2|  
  |program3|得分3|
  |rate3|占比3|
  |comment3|评价3|
   |program4|得分4|
  |rate4|占比4|
  |comment4|评价4|
  |program5|得分5|
  |rate5|占比5|
  |comment5|评价5|
  |update_date|评测时间|  
 
- 返回实例：

        {         
            "status": true,
            "info": null
        }

- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|


