## 流程图1：考试及成绩管理流程

**PlantUML源码如下：**

```
@startuml

:安排考试;

:考试安排表;

:出卷;

fork

:A试卷;

fork again

:B试卷;

fork again

:打印审批表;

:审批签字;

endfork

:打印试卷;

:试卷;

:参加考试;

:答卷;

:阅卷出成绩;

fork

:答卷;

:装订存档;

fork again

if(是否有不及格)then(有)

:安排补考;

:补考安排表;

else()

stop

endif

endfork

:期末流程结束;

@enduml

```

**业务流程图如下：**

![1](C:\Users\12345\Desktop\test1\1.png)

## 流程图2： 客户维修服务流程

**PlantUML源码如下：**

```
@startuml
start
:申请服务;
if(新客户)then(是)
:登记客户信息;
:上门勘察;
else()
:上门勘察;
endif
:制定方案;
if(满意)then(是)
:签订服务合同;
else(否)
stop
endif
fork
:安排工人;
fork again
:安排材料;
endfork
:填写派工单;
:领取材料;
:上门服务;
:验收并填写反馈意见;
:交回派工单;
:结算收款;
stop
@enduml
```

**业务流程图如下：**

![2](C:\Users\12345\Desktop\test1\2.png)