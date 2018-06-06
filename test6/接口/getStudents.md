#### 用例： 学生列表
- 权限： 学生/老师都能看到列表，访客不能看到列表。
- 功能： 返回所有学生的列表。
- API请求地址： 接口基本地址/v1/api/getStudents
- 请求方式 ： GET
- 请求参数说明: 无
```
 {
      "status": true,
      "info": "获取结果成功",
      "total": 51,
      "data": [
          {
          "GITHUB_ NAME": "luojiajie",
          "ID":11,
          "STUDENT_NO": "201510414211",
          "STUDENT_CLASS": "软件(本)15-2",
          "STUDENT_NAME": "罗家杰",
          "STATUS":"6",
          "ADDTIME": "2018-06-06 14:48:01",
          "TERM_ID":6,
          "GRADE_ID":6,
          "TEST_ID":6,
          "COURSE_NO":25,
          "GRADE_1":90,
          "GRADE_2":95,
          "GRADE_3":90,
          "MOME":"这个同学完成度不错",
          ...
          },
          
          {
          ...其他学生
          }
      ]
  }

```
- 返回参数说明：

	数名称	| 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息
total |返回学生人数
data | 所有学生的数组
	STUDENT_GITHUB_ NAME | 学生的GITHUB 用户名 
STUDENT_NO | 学号
STUDENT_NAME | 真实姓名
ADDTIME | 增加日期
ID | 数据库自增 
STATUS | 是否正常
TERM_ID | 学期编号
GRADE_ID | 成绩编号
TEST_ID | 实验编号
COURSE_NO | 课程编号
GRADE_1 | 完成度分数1 
GRADE_2 | 总体结构分数2 
GRADE_3 | 实验报告分数3 
MOME | 评价
