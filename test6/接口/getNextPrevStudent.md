# 接口：getNextPrevStudent [返回](https://github.com/lk357293221/is_analysis/blob/master/test6/README.md)

用例：[评定成绩](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E8%AF%84%E5%AE%9A%E6%88%90%E7%BB%A9.md)

- 功能：返回一个学生的上一个或者下一个学生的学号。

- 权限：
  老师：只有老师可以调用该API。

- API请求地址：接口基本地址/ v1 / api / getNextPrevStudent / <is_next> / <student_id>

- 请求方式：GET

- 请求参数说明：

  | 参数名称 | 说明                                                         |
  | -------- | ------------------------------------------------------------ |
  | is_next  | 是下一个还是上一个，如果为1表示取下一个学生，如果为0表示上一个学生 |
  | 学生卡   | 学生的学号                                                   |

- 返回实例：

  ```
    {         
        "status": true,
        "info": null,    
        "student_id": "201510414212"
    }
  ```

- 返回参数说明：

  | 参数名称 | 说明                                       |
  | -------- | ------------------------------------------ |
  | 状态     | 布尔类型，真表示正确的返回，虚假表示有错误 |
  | 信息     | 返回结果说明信息                           |
  | 学生卡   | 学号                                       |