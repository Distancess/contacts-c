﻿# WonderLand ApiDoc - User

标签（空格分隔）： WonderLand

---

## **日志**

| 日期         | 备注  
| ------------ | ------
| **17/10/23** | 新增接口 · **【用户登录 login】**


---

## **属性**

- **【user 表】**

| 属性名        | 中文   | 最小长度 | 最大长度 | 类型      | 特殊要求
| ------------- | ------ | -------- | -------- | --------- | --------
| **Uusername** | 用户名 | 6        | 16       | char(20)  | 字母/数字/下划线/破折号
| **Upassword** | 密码   | 6        | 16       | char(20)  | -                     
| **Utype**     | 类型   | -        | -        | -         | - 
| **Utoken**    | 凭据   | 30       | 30       | char(30)  | -
| **Ulast_visit**| 上次访问 | -     | -        | TIMESTAMP | - 

---

## **接口 · 登陆**

- **请求方法：POST**
- **接口网址：http://contacts-c.and-who.cn/User/login**

- **表单要求**

| 属性名        | 必要性 | 最小长度 | 最大长度 | 特殊要求
| ------------- | ------ | -------- | -------- | --------
| **Uusername** | O      | -        | -        | - 
| **Upassword** | O      | -        | -        | -


- **成功返回**

```
{
	"type": 1,
	"message": "登陆成功",
	"data": {
		"学号": "xxxxxx",
		"姓名": "xxx",
		"本人电话": "xxxxxxx",
		"家庭住址": "xxxxxxx",
		"Utoken": "J8FPzEVUyiYl6LdR5rSnXbZCgWMwAt"
	}
}
```

