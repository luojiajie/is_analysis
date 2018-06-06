#### 用例： 分数列表
- 权限： 学生/老师登录后可以看到,访客不能看到。
- 功能： 返回所有分数的列表。
- API请求地址： 接口基本地址/v1/api/getGrades
- 请求方式 ： GET
- 请求参数说明: 无
```
 {
      "status": true,
      "info": "获取结果成功",
      "total": 36,
      "data": [
          {
          "GRADE_ID":2,
          "COURSE_NO":"41052",
          "STUDENT_NO":"201510414211",
          "TEST_ID":"15",
          "GRADE_1":90,
          "GRADE_2":95,
          "GRADE_3":90,
          "MOME":"这个同学完成度不错",
          "ADDTIME": "2018-06-06 14:48:01",
          ...
          },
          
          {
          ...其他分数
          }
      ]
  }

```
- 返回参数说明：

	数名称	| 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息
total |返回分数数量
data | 所有分数的数组
	RADE_ID | 教师创建 
COURSE_NO |课程编号
STUDENT_NO |学生编号
TEST_ID |实验编号
GRADE_1| 完成度分数1 
GRADE_2| 总体结构分数2 
GRADE_3| 实验报告分数3 
MOME|评价
ADDTIME | 增加日期


