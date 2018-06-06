#### 用例： 查看成绩、评定成绩
- 权限：学生：只能查看自己的成绩，即接口参数stu_no必须等于登录学生的stu_no 老师：可以查看所有学生的成绩。
- 功能： 返回一个学生的所有实验成绩和实验评价。
- API请求地址： 接口基本地址/v1/api/getOneStudentResults/<term_id>/<course_no>/<test_id>/<stu_no>
- 请求方式 ： GET
- 请求参数说明: 

参数名称 | 说明
---|---
term_id | 学期编号
course_no| 课程编号
test_id| 实验编号
student_no| 学生编号
- 返回实例：
```
  {         
      "status": true,
      "info": "返回结果成功",    
      "STUDENT_NO": "201510414211", 
      "GITHUN_NAME": "luojiajie", 
      "STUDENT_CLASS": "软件(本)15-2", 
      "STUDENT_NAME": "罗家杰", 
      "total": 6,
      "data": [
          {
          "GRADE_ID":1,
          "TEST_ID": "51", 
          "COURSE_NO": "41051", 
          "STUDENT_NO":"201510414211",
          "GRADE_1":90,
          "GRADE_2":95,
          "GRADE_3":90,
          "MOME":"本实验做得好",
          "ADDTIME": "2018-06-06 14:48:01"
          }
      ] 
  }

```
- 返回参数说明：

	数名称	| 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息
STUDENT_NO |学生编号
STUDENT_GITHUN_NAME |学生的GITHUB用户名
STUDENT_CLASS |学生班级
STUDENT_NAME |学生姓名
total |返回记录
data |返回结果的数组
GRADE_ID| 分数编号
TEST_ID |实验编号
COURSE_NO |课程编号
STUDENT_NO |学生编号
GRADE_1 |完成度分数1
GRADE_2 |总体结构分数2
GRADE_3 |实验报告分数3
MOME |评价
ADDTIME |新增时间



