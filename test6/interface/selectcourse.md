# 接口：selectcourse  [返回](../README.md)
用例： [选择课程](../usecaseprinciple/student_course_select.md)

- 功能：
    选择课程。
    
- 权限：
    学生。    
    
- API请求地址： 
    接口基本地址/v1/api/selectcourse

- 请求方式 ：
    POST

- 请求实例：

        {
            "course_id":"222048329823",
            "student_id":"12",
        }
        
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |course_id|课程id|
  |student_id|学生id| 
  
- 返回实例：
        
        {
            "status": 1,
            "info": "成功",
            "data": ""
        }

- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |data|返回的数据|