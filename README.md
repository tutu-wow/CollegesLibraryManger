# CollegesLibraryManger
图书管理系统 计算机毕业设计 角色：学生、教师、管理员；亮点：AI助手、协同过滤算法、腾讯地图api、Echarts图形化分析、二维码识别；

所有源码均本人开发，项目是前后端分离的，所有的项目都具备了完整的业务逻辑，不仅仅局限于基础的增删改查（CRUD）操作，系统亮点众多。

本文注重于计算机毕业设计选题指导，列出题目均有源码， 大家可以去【公众号】(毕业终点站)获取或者加我【qq】(2112698948)提意见(别忘记Star哟)。备注：git

声明：仅用于学习使用，请勿用于任何商业行为！

1.系统非商用，非开源，非无偿。

2.由本人开发，如需源码，请联系以下方式，qq:2112698948。

3.项目有很多，并未全部上传，如果未找到想要的，可直接咨询。
<font style="color:#117cee;">🎈</font><font style="color:#117cee;">系统亮点：AI助手、协同过滤算法、腾讯地图api、Echarts图形化分析；、二维码识别</font>

# <font style="color:#48b378;">一.系统开发工具与环境搭建</font>
## <font style="color:#262626;">1.系统设计开发工具</font>
<font style="color:#262626;">后端使用Java编程语言的Spring boot框架</font>  
<font style="color:#262626;">项目架构：B/S架构</font>  
<font style="color:#262626;">运行环境：win10/win11、jdk17</font>



<font style="color:#48b378;">前端：</font>  
<font style="color:#262626;">技术：框架Vue3 ；UI库：Element-Plus；</font>  
<font style="color:#262626;">开发工具：Visual Studio Code；</font>

---

<font style="color:#48b378;">后端:</font>  
<font style="color:#262626;">技术：Java语言、mybatis-plus、Spring boot框架；</font>  
<font style="color:#262626;">开发工具：IDEA 2025版本；</font>

---

<font style="color:#48b378;">数据库：</font>  
<font style="color:#262626;">数据库：mysql5.7/8.0 </font>  
<font style="color:#262626;">数据库工具：Navicat12版本；</font>

---

# <font style="color:#48b378;">二.系统实现</font>
高校图书馆预约管理系统有三个角色，学生、教师和管理员。是一套围绕“图书馆区域、自习室座位、预约规则、学习资讯、积分记录、消息通知和 AI 自习推荐”构建的学习空间预约平台。系统既覆盖后台座位和规则管理，也覆盖前台预约、扫码、学习时长和积分记录，适合展示图书馆预约类项目。

## <font style="color:#222222;">业务流程</font>
**<font style="color:#222222;">空间建档流程</font>**<font style="color:#222222;">：后台维护图书馆区域、房间、座位和预约规则，形成可预约的学习空间资源。</font>

**<font style="color:#222222;">预约流程</font>**<font style="color:#222222;">：用户浏览房间详情后选择座位提交预约，系统记录预约状态和预约时段，并支持超时记录追踪。</font>

**<font style="color:#222222;">学习使用流程</font>**<font style="color:#222222;">：用户在使用过程中通过扫码或使用页面完成学习时长沉淀，系统累计个人学习数据。</font>

**<font style="color:#222222;">积分沉淀流程</font>**<font style="color:#222222;">：系统根据预约和学习行为生成积分记录，用户在前台查看积分明细和积分来源。</font>

**<font style="color:#222222;">资讯互动流程</font>**<font style="color:#222222;">：平台发布图书馆资讯内容，用户阅读文章并沉淀浏览、点赞、收藏等行为数据。</font>

**<font style="color:#222222;">核心业务闭环</font>**<font style="color:#222222;">：平台围绕“空间建档 - 座位预约 - 使用扫码 - 学习时长与积分沉淀 - 资讯互动 - 统计分析”形成图书馆预约闭环。</font>

## 2.1 学生
### 2.1.1 首页
推荐资讯为协同过滤算法推荐。

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985990744-bd61a07a-8872-4611-bd3d-d41fc01c073f.png)

### 2.1.2 图书馆选座
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985991797-2954f37a-04a7-49ad-a0c4-f52541c2d817.png)

### 2.1.3 可视化座位
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985990107-82b8a6b2-c401-4590-95cb-dcc0711d9325.png)

### 2.1.4 AI助手
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985987967-7a923bab-e483-4f8e-8904-15fbfd4a4acd.png)

### 2.1.5 区域介绍
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985991570-31b4a1a3-fc6f-4d53-b655-31acf2a09ef5.png)

### 2.1.5 座位监督
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985990852-961847cf-96a2-4baa-aa96-fd4c2ce84000.png)

### 2.1.6 文章资讯
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985991419-dc8a3e56-ffcd-4656-ac52-647fee36ddbe.png)

### 2.1.7 资讯详情
相关推荐为协同过滤算法推荐。

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985998961-f8379ead-842b-45b2-a9d1-bd7eee476d06.png)

### 2.1.8 预约记录
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985998401-edcd4204-40f0-4f64-ad44-15c846d794a5.png)

### 2.1.9学习统计
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985998837-dc70b975-5c97-453c-9ff6-f59f6fec3d63.png)

### 2.1.10 积分记录
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985998984-df7fcf51-3392-4760-aa07-593918d17f28.png)

## 2.2 教师
### 2.2.1 学生列表
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784985999234-faf5e46b-eb8e-4c1c-b41f-0dd189d2c6c3.png)

## 2.3 管理员
### 2.3.1 积分统计
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986004300-38e828b3-565e-4fe9-9cc4-5292d432fe45.png)

### 2.3.2 老师信息
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986006266-cb0fafc2-688f-47f6-ae56-145f3c2d153f.png)

### 2.3.3 图书馆管理
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986006410-cf833250-c415-40f3-b7f7-d46d48e1fac3.png)

### 2.3.4 预约配置
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986006627-7c1c1ccd-9325-4b45-bf4f-8cd17b4d36c5.png)

### 2.3.5 座位管理
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986006725-88904ad7-0bd8-4b4c-abdd-df20d92bf73e.png)

### 2.3.6 预约记录
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986007400-10ab7823-fe6f-4d0f-9618-930a6ce23762.png)

### 2.3.7 积分记录
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986008236-d3a3d1a5-f2ac-4a49-81c1-e15a214c0f52.png)

### 2.3.8 文章管理
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986013915-5ea3b036-3c7f-4a3f-bb5d-af75d3f7864e.png)

### 2.3.9 文章统计
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986014114-6bbf7090-9740-4580-aa32-830b0a5d2d03.png)



# <font style="color:#48b378;">三.系统代码结构截图</font>
## <font style="color:#262626;">3.1 前端</font>
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986014333-8051e3b7-0b93-4b13-82c0-5192fee7369e.png)

## 3.2 后端
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986015262-38635866-f907-4718-a9bd-68b37d6a879c.png)

## 3.3 数据库
18张数据库

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784986012211-f605d66e-25fc-408e-b07b-2ebf7c491162.png)

# <font style="color:#48b378;">四.</font><font style="color:#1aad19;">源码获取</font>
<font style="color:#000000;">1.原创系统非商用，非开源，非无偿。</font>

<font style="color:#000000;">2.项目有很多，并未全部上传，如果未找到想要的，可直接咨询。</font>

