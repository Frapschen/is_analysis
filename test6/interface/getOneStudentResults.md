<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getOneStudentResults  [返回](../README.md)
用例： [查看成绩](../usecaseprinciple/inquiry.md)，[评定成绩](../usecaseprinciple/evaluate_grades.md)

- 功能：
    返回一个学生的所有实验成绩和实验评价。
    
- 权限：
    学生：只能查看自己的成绩，即接口参数student_id必须等于登录学生的student_id
    老师：可以查看所有学生的成绩。
    
- API请求地址： 
    接口基本地址/v1/api/getOneStudentResults/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |student_id|学生的学号|
  |course_id|课程编号|
    
- 返回实例：

        {
        "status": true,
        "code": 200,
        "data": {
            "student_id": "201510315203",
            "github_username": "chinajuedui",
            "total": 6,
            "avgresult": 90.5,
            "tests": [{
                    "test_id": 1,
                    "web_exists": true,
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
                    "memo": "本实验做得好",
                    "update_date": "2018-04-02 13:48:01"
                },
                {...其他实验}
            ]
        }
}
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |code|返回代码|
  |student_id|学号|
  |github_username|学生的gitHub用户名|  
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
  |web_exists|本实验的GitHub网页是否存在|
  |result|本实验成绩，可以为空，为空表示没有批改，没有批改的实验不入平均成绩，为0分则要计入平均成绩，所以成绩为空和为0是不一样的。|
  |update_date|本实验老师的批改日期，可以为空|


