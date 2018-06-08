# 接口：getStudents [返回](https://github.com/lk357293221/is_analysis/blob/master/test6/README.md)

用例：[学生列表](https://github.com/lk357293221/is_analysis/blob/%E5%AD%A6%E7%94%9F%E5%88%97%E8%A1%A8.md)

- 权限：学生/访客：不能看到RESULT_SUM，WEB_SUM老师：可以看到RESULT_SUM，WEB_SUM。

- 功能：返回所有学生的列表。

- API请求地址：接口基本地址/ v1 / api / getStudents

- 请求方式：GET

- 请求参数说明：无

- 返回实例：

  ```
    {
        "status": true,
        "info": null,
        "total": 121,
        "data": [
            {"WEB_SUM": "Y,Y,Y,Y,Y,N",
            "RESULT_SUM": "83.75,90,80,80,85,N",
            "GITHUB_USERNAME": "Chinajuedui",
            "STUDENT_ID": "201510414212",
            "CLASS": "软件(本)15-2",
            "NAME": "罗凯",
            "UPDATE_DATE": "2018-04-02 13:48:01"},
            {
            ...其他学生
            }
        ]
    }
  ```

  返回参数说明：

  | 参数名称        | 说明                                       |
  | --------------- | ------------------------------------------ |
  | 状态            | 布尔类型，真表示正确的返回，虚假表示有错误 |
  | 信息            | 返回结果说明信息                           |
  | 总              | 返回学生人数                               |
  | 数据            | 所有学生的数组                             |
  | WEB_SUM         | 网址是否正确的汇总                         |
  | RESULT_SUM      | 成绩的汇总                                 |
  | GITHUB_USERNAME | GITHUB用户名                               |
  | 学生卡          | 学号                                       |
  | 类              | 班级                                       |
  | 名称            | 真实姓名                                   |
  | 更新日期        | GitHub的用户名修改日期                     |

  ​