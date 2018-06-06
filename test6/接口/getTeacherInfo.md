#### 用例： 老师信息
- 权限： 学生不能查看 、 老师登录后可以看到。
- 功能： 返回对应老师的信息。
- API请求地址： 接口基本地址/v1/api/getTeacherInfo/<tch_no>
- 请求方式 ： GET
- 请求参数说明: 

请求参数 | 说明
---|---
teacher_no | 老师编号

```
 {
      "status": true,
      "info": "获取结果成功",
      "data": 
          {
          "GITHUB_ NAME": "Mr Zhao",
          "ID":19,
          "TEACHER_NO": 514211",
          "TEACHER_NAME": "赵老师",
          "STATUS":"1",
          "ADDTIME": "2018-06-06 14:48:01",
          "TERM_ID":2
          ...
          }
  }

```
- 返回参数说明：

	数名称	| 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息
data | 所有老师的信息集合
	TEACHER_GITHUB_ NAME | 老师的GITHUB 用户名 
TEACHER_NO |实验编号
TERM_ID | 学期编号
TEACHER_NAME | 真实姓名
ADDTIME | 增加日期
ID | 教师创建 
STATUS | 是否正常

