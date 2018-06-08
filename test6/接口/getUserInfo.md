# 接口：getUserInfo [返回](https://github.com/lk357293221/is_analysis/blob/master/test6/README.md)

用例：[查看用户信息](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E6%9F%A5%E7%9C%8B%E7%94%A8%E6%88%B7%E4%BF%A1%E6%81%AF.md)，[修改用户信息](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E4%BF%AE%E6%94%B9%E7%94%A8%E6%88%B7%E4%BF%A1%E6%81%AF.md)

- 功能：查看用户的所有信息。

- 权限：学生/老师：查看自己的信息，必须先登录，不能查看其他用户的信息。

- API请求地址：接口基本地址/ v1 / api / getUserInfo / <user_id>

- 请求方式：GET

- 请求参数说明：

  | 参数名称 | 说明                                |
  | -------- | ----------------------------------- |
  | 用户名   | 用户的ID号。对应表USERS.USER_ID的值 |

- 返回实例：

  ```
    {         
        "status": true,
        "info": null,
        "ID":"201510414212",    
        "name":"罗凯",
        "class_dept":"软件工程2班"
        "github_username":"ABCD",
        "type":"学生"            
    }
  ```

- 返回参数说明：

  | 参数名称        | 说明                                       |
  | --------------- | ------------------------------------------ |
  | 状态            | 布尔类型，真表示正确的返回，虚假表示有错误 |
  | 信息            | 返回结果说明信息                           |
  | ID              | 学号或者工号                               |
  | 名称            | 用户的真实姓名                             |
  | class_dept      | 班级或者部门名称                           |
  | github_username | GitHub的用户名                             |
  | 类型            | 用户类型：老师或者学生                     |