---
title: 快速开始
category: Nirvana
order: 6
---

## 登录
Nirvana 登录页面点击 “Get Gitlab Authority”，页面跳转值 GitLab 登录页面，输入 GitLab 用户信息并登录，进入Nirvana主页面。


## 添加Repo
点击 “Add Repo” 按钮，弹出界面选择要测试的项目并且确认。主页面将展示新增的 Repo 信息。    

## 添加变量

#### 环境变量  
`host`为请求的服务地址，环境变量中必须有 host 且仅在环境变量中有效。  
1.进入 Repo，选择接口文档，Nirvana会将符合 swagger 3.0 规范的 yaml 转换为接口信息展示。  
2.点击 “Variable”，进入环境变量添加界面。  
3.点击 Envs 右侧 “+”按钮，创建环境*（在实际测试中会有多套环境，包括测试环境、预生产环境、或者针对不同版本的环境，每个环境对应的一些变量如请求地址、用户信息和中间件地址等都不相同，为了避免每测试一个环境都要手动修改相关数据，引入环境概念）。*  
4.在环境中添加变量（ host 变量为必须），并提供环境变量的启、禁用功能。  

#### 全局变量  
项目界面，点击  “Global Variable” 按钮，弹出全局变量界面。  


## 测试用例管理  


#### 添加测试用例   
1.项目界面，切换至 Swagger 界面，点击 “Test Case” 按钮，进入测试用例管理界面。  
2.Nivarna 会根据接口文档自动生产测试用例模版.  
3.输入用例标题、描述，输入接口请求头、请求体参数，添加 Response 断言，点击 “Save” 按钮，测试用例添加成功。  
引用环境变量用符号 “$”，如 $Key。  
4.点击 “Creat” 按钮可以再次添加用例。或者点击“复制”按钮，复用已添加的用例。  


#### 执行测试用例  
1.测试用例管理界面，选择需要执行的测试用例，点击左上角 “Run” 按钮。  
2.进入到环境选择界面，根据选择的环境对应展示具体的变量信息。  
3.点击右上角 “Run”，开始执行测试用例并展示执行结果。  
4.Nirvana 提供完整的日志信息，可点击结果界面的 “log” 按钮。  
5.结果界面也可以切换环境多次执行测试用例。  








