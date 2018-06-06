#### 用例： 修改老师信息
- 权限：学生/老师：修改自己的信息，必须先登录。
- 功能： 修改老师的基本信息。
- API请求地址： 接口基本地址/v1/api/setPassword/<tch_no>
- 请求方式 ： post
- 请求实例：

```
  {         
      "teacher_no":"201510414213",
      "data": 
          {
          "GITHUB_ NAME": "Mr Zhao",
          "ID":15,
          "STUDENT_NO": "201510414211",
          "STUDENT_NAME": "赵老师",
          "STATUS":"1",
          "ADDTIME": "2018-06-06 14:48:01",
          ...
          }
  }

```
- 请求参数说明：

	数名称	| 说明
---|---
teacher_no|老师学号
data | 老师信息集合
ID|数据库自增
	TEACHER_GITHUB_ NAME | 老师的GITHUB 用户名 
TEACHER_NO | 老师编号
TEACHER_NAME | 真实姓名
STATUS|是否正常
ADDTIME | 增加日期

- 返回实例：
```
{         
      "status": true,
      "info": "修改成功"
  }
```


参数名称 | 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息


