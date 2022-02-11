### 项目介绍

这是一个采用前后端分离开发的项目，前端采用 vue 开发、后端采用 spring boot 开发。



#### 项目展示

1. 登陆界面

![image-20220211152715838](README.assets/image-20220211152715838.png)

2. admin 主界面

![image-20220211152913239](README.assets/image-20220211152913239.png)

3. 动态搜索框与表格展示

![image-20220211153012483](README.assets/image-20220211153012483.png)

4. 学生端首页展示

![image-20220211153053836](README.assets/image-20220211153053836.png)

5. 教师端成绩搜索与编辑

![image-20220211153257252](README.assets/image-20220211153257252.png)

### 前端部分

#### 项目运行

**由于涉及大量的 ES6/7 等新属性，node 需要 6.0 以上版本**

```shell
git clone git@github.com:ruanjiancheng/StudentManageSystem.git

cd /StudentManageSystem/student_client

npm install

npm run serve
```

#### 技术栈

- vuex
- router
- axios
- element ui

#### 项目介绍

采用 vue 2.0 开发,通过调用后端提供的数据接口实现数据的动态渲染.

- 使用监视器,以及得益于 Mybatis 提供动态 SQL 功能,实现动态搜索功能
- 同时实现了基于前端和后端的数据分页功能
- 使用 router 配置路由,实现不同用户类型导航栏的动态渲染
- 使用 axios 异步加载后端数据
- 使用 element ui 实现表单的前端校验功能

#### 实现的功能

1. admin
   1. 实现对教师, 学生, 课程的 CRUD
   2. 实现对教师业务以及学生业务的全方位控制
2. teacher 
   1. 实现查询我开设的课程, 以及选择我课程的学生信息
   2. 对学生成绩的登陆
3. student
   1. 实现选课退课的功能
   2. 实现成绩查询的功能



### 后端部分

#### 项目运行

```shell
git clone git@github.com:ruanjiancheng/StudentManageSystem.git

cd /StudentManageSystem/student_server

java -jar student_server-0.0.1-SNAPSHOT.jar

```

#### 技术栈

- spring boot
- Mybatis
- JDBC
- Lombok

#### 项目介绍

采用 Restful 风格开发,采用 CrossOrigin 解决跨域问题. 采用注解以及 xml 文件配置 SQL 语句, 实现动态 SQL 的功能.



### 项目存在的问题

- 由于是第一次编写 Vue 项目, 代码复用做得并不是很好. 导致许多组件代码量巨大. 

- 期间多次因为太菜了, 导致功能实现不了. 感谢博客园的大佬相助. (CSDN 狗都不用)