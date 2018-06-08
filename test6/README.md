## 1.概述

- 基于GitHub的实验管理平台的作用是在线管理实验成绩的Web应用系统。学生和老师的实验内容均存放在GitHUB页面上。
- 学生的功能主要有：一是设置自己的GitHub的用户名，二是查询自己的实验成绩学生的GitHub的用户名是公开的，但成绩不公开。
- 老师的功能主要有：一是批改每个学生的成绩，二是查看每个学生的成绩。
- 老师和学生都能通过本系统的链接方便地跳转到学生的每个github上实验目录，以便批改实验或者查看实验情况。
- 实验成绩按数字分数计算，每项实验的满分为100分，最低为0分。
- 系统自动计算每个学生的所有实验的平均分。

## 2.系统总体结构

[![img](https://github.com/lk357293221/is_analysis/raw/master/test6/%E7%B3%BB%E7%BB%9F%E6%80%BB%E4%BD%93%E7%BB%93%E6%9E%84.png)](https://github.com/zwdbox/is_analysis/blob/master/test6/%E7%B3%BB%E7%BB%9F%E6%80%BB%E4%BD%93%E7%BB%93%E6%9E%84.png)

界面设计参见：[https](https://zwdbox.github.io/is_analysis/test6/ui/index.html)：//lk357293221.github.io/is_analysis/test6/ui/index.html

## 3.用例图设计[源码](https://github.com/lk357293221/is_analysis/blob/master/test6/src/UseCase.puml)

[![img](https://github.com/lk357293221/is_analysis/raw/master/test6/UseCase.png)](https://github.com/zwdbox/is_analysis/blob/master/test6/UseCase.png)

## 4.类图设计[源码](https://github.com/lk357293221/is_analysis/blob/master/test6/src/class.puml)

[![img](https://github.com/lk357293221/is_analysis/raw/master/test6/class.png)](https://github.com/zwdbox/is_analysis/blob/master/test6/class.png)

## 5.数据库设计

- ### [参见数据库设计](https://github.com/lk357293221/is_analysis/blob/master/test6/%E6%95%B0%E6%8D%AE%E5%BA%93%E8%AE%BE%E8%AE%A1.md)

## 6.用例和界面详细设计

- ### [“学生列表”用例](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E5%AD%A6%E7%94%9F%E5%88%97%E8%A1%A8.md)，[界面](https://lk357293221.github.io/is_analysis/test6/ui/index.html)

- ### [“评定成绩”用例](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E8%AF%84%E5%AE%9A%E6%88%90%E7%BB%A9.md)，[界面](https://lk357293221.github.io/is_analysis/test6/ui/%E8%AF%84%E5%AE%9A%E6%88%90%E7%BB%A9.html)

- ### [“查看成绩”用例](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E6%9F%A5%E7%9C%8B%E6%88%90%E7%BB%A9.md)，[界面](https://lk357293221.github.io/is_analysis/test6/ui/%E6%9F%A5%E7%9C%8B%E6%88%90%E7%BB%A9.html)

- ### [“修改密码”用例](https://lk357293221/zwdbox/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E4%BF%AE%E6%94%B9%E5%AF%86%E7%A0%81.md)，[界面](https://lk357293221.github.io/is_analysis/test6/ui/%E9%A1%B6%E9%83%A8%E8%8F%9C%E5%8D%95.html)

- ### [“修改用户信息”用例](https://lk357293221/zwdbox/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E4%BF%AE%E6%94%B9%E7%94%A8%E6%88%B7%E4%BF%A1%E6%81%AF.md)，[界面](https://lk357293221.github.io/is_analysis/test6/ui/%E9%A1%B6%E9%83%A8%E8%8F%9C%E5%8D%95.html)

- ### [“查看用户信息”用例](https://lk357293221/zwdbox/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E6%9F%A5%E7%9C%8B%E7%94%A8%E6%88%B7%E4%BF%A1%E6%81%AF.md)，[界面](https://lk357293221.github.io/is_analysis/test6/ui/%E9%A1%B6%E9%83%A8%E8%8F%9C%E5%8D%95.html)

- ### [“登出”用例](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E7%99%BB%E5%87%BA.md)，[界面](https://lk357293221.github.io/is_analysis/test6/ui/%E9%A1%B6%E9%83%A8%E8%8F%9C%E5%8D%95.html)

- ### [“登录”用例](https://github.com/lk357293221/is_analysis/blob/master/test6/%E7%94%A8%E4%BE%8B/%E7%99%BB%E5%BD%95.md)，[界面](https://lk357293221.github.io/is_analysis/test6/ui/%E7%99%BB%E5%BD%95.html)