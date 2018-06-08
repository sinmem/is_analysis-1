# 接口：setUserInfo [返回](https://github.com/lk357293221/is_analysis/blob/master/test6/README.md)

用例：[修改用户信息](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E4%BF%AE%E6%94%B9%E7%94%A8%E6%88%B7%E4%BF%A1%E6%81%AF.md)

- 功能：修改用户的GitHub用户名。

- 权限：学生/老师：修改自己的密码，必须先登录。

- API请求地址：接口基本地址/ v1 / api / setUserInfo

- 请求方式：POST

- 请求实例：

  ```
    {
        "id":"21048329823",
        "github_username":"ABCDE",            
    }
  ```

- 请求参数说明：

  | 参数名称        | 说明                                |
  | --------------- | ----------------------------------- |
  | 用户名          | 用户的ID号。对应表USERS.USER_ID的值 |
  | github_username | 用户GitHub的用户名。                |

- 返回实例：

  ```
    {         
        "status": true,
        "info": null
    }
  ```

- 返回参数说明：

  | 参数名称 | 说明                                       |
  | -------- | ------------------------------------------ |
  | 状态     | 布尔类型，真表示正确的返回，虚假表示有错误 |
  | 信息     | 返回结果说明信息                           |