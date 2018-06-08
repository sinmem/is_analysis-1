# 接口：getOneStudentResults [返回](https://github.com/lk357293221/is_analysis/blob/master/test6/README.md)

用例：[查看成绩](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E6%9F%A5%E7%9C%8B%E6%88%90%E7%BB%A9.md)，[评定成绩](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E8%AF%84%E5%AE%9A%E6%88%90%E7%BB%A9.md)

- 功能：返回一个学生的所有实验成绩和实验评价。

- 权限：学生：只能查看自己的成绩，即接口参数student_id必须等于登录学生的student_id老师：可以查看所有学生的成绩。

- API请求地址：接口基本地址/ v1 / api / getOneStudentResults / <student_id>

- 请求方式：GET

- 请求参数说明：

  | 参数名称 | 说明       |
  | -------- | ---------- |
  | 学生卡   | 学生的学号 |

- 返回实例：

  ```
    {         
        "status": true,
        "info": null,    
        "student_id": "201510414212", 
        "github_username": "chinajuedui", 
        "class": "软件(本)15-2", 
        "name": "罗凯", 
        "total": 6,
        "avgresult":90,       
        "data": [
            {
            "test_id":1,
            "web_exists": true, 
            "result": 91, 
            "memo":"本实验做得好",
            "update_date": "2018-04-02 13:48:01"
            }, 
            {
            ...其他实验
            }
        ] 
    }
  ```

- 返回参数说明：

  | 参数名称        | 说明                                                         |
  | --------------- | ------------------------------------------------------------ |
  | 状态            | 布尔类型，真表示正确的返回，虚假表示有错误                   |
  | 信息            | 返回结果说明信息                                             |
  | 学生卡          | 学号                                                         |
  | github_username | 学生的GitHub的用户名                                         |
  | 类              | 班级                                                         |
  | 名称            | 真实姓名                                                     |
  | 总              | 实验总数                                                     |
  | avgresult       | 实验平均成绩                                                 |
  | 数据            | 所有实验的成绩和评语                                         |
  | 为test_id       | 实验编号                                                     |
  | web_exists      | 本实验的GitHub的网页是否存在                                 |
  | 结果            | 本实验成绩，可以为空，为空表示没有批改，没有批改的实验不入平均成绩，为0分则要计入平均成绩，所以成绩为空和为0是不一样的。 |
  | 备忘录          | 本实验老师的评价，可以为空                                   |
  | 更新日期        | 本实验老师的批改日期，可以为空                               |