<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setUserInfo  [返回](../README.md)
用例： [修改用户信息](../usecaseprinciple/modify_userInfor.md)

- 功能：
    修改用户的GitHub用户名。
    
- 权限：
    学生/老师：修改自己用户信息，必须先登录。    
    
- API请求地址： 
    接口基本地址/v1/api/setUserInfo

- 请求方式 ：
    POST

- 请求实例：

        {
            "id":"21048329823",
            "github_username":"ABCDE",
            "email":"1290130117@qq.com",
             "phone":"18200244217",
             "name": "张三",
             "class_dept": "软件工程1班",
             "type": "学生"            
        }
        
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |user_id|用户的ID号。对应表USERS.USER_ID的值|
  |github_username|用户GitHub用户名。|
  |email|邮箱。|
  |phone|电话号码。|
  |name|姓名。|
  |class_dept|专业班级。| 
  
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


