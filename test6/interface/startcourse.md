# 接口：startcourse  [返回](../README.md)
用例： [开课](../usecaseprinciple/start_course.md)

- 功能：
    开启一个新的课程。
    
- 权限：
    老师。    
    
- API请求地址： 
    接口基本地址/v1/api/startcourse

- 请求方式 ：
    POST

- 请求实例：

        {
            "teacher_id":"222048329823",
            "name"："数据库",
            "term"："大二下",
            "num":60,
            "totaltest":5,
            "dateline":"2020-5-27 23:00",
            "introduce":"简介"
        }
        
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |teacher_id|老师的工号|
  |name|课程名字|
  |term|学期|
  |num|学生总人数|
  |totaltest|实验次数|
  |datalien|选课截止时间|
  |introduce|课程简介|
              
  
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