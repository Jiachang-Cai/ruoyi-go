# Go版Java若依(目前暂不开源)

## 功能模块
| 功能点 | 完成状态 |
|-----|------|
| 自定义错误消息 | 完成   |
| 公共JSON响应体 | 完成   |
| 初始化配置文件 | 完成   |
| 初始化数据库(多个) | 完成   |
| 初始化Redis(多个) | 完成   |
| 初始化日志 | 完成   |
| 优雅重启或停止 | 完成   |
| 自定义gorm.Model | 完成   |
| 根据struct tag 动态拼接 Gorm where | 完成   |
| 图形验证码生成与校验(redis) | 完成   |
| redis操作工具 | 完成   |
| RSA加解密工具 | 完成   |
| Jwt工具 | 完成   |
| excel工具 | 完成   |
| 请求参数sign校验 | 完成   |
| 操作日志中间件 | 完成   |
| jwt校验中间件(redis) | 完成   |
| 登录并拉取角色菜单权限 | 完成   |
| 登录密码错误次数限制 | 完成   |
| 数据权限(根据不同表特殊处理) | 完成   |
| 接口访问权限 | 完成   |
| 用户管理 | 完成   |
| 个人中心 | 完成   |
| 角色管理 | 完成   |
| 菜单管理 | 完成   |
| 部门管理 | 完成   |
| 岗位管理 | 完成   |
| 字典管理 | 完成   |
| 参数设置 | 完成   |
| 通知公告 | 完成   |
| 操作日志 | 完成   |
| 登录日志 | 完成   |
| 在线用户 | 完成   |
| 服务监控 | 完成   |
| 缓存监控 | 完成   |
| 缓存列表 | 完成   |
| 定时任务 | 完成   |
| 数据监控 | 第三方插件不考虑   |
| 表单构建 | 纯页面非后端   |
| 代码生成 | 暂不处理   |
| 系统接口 | swagger支持 暂不处理   |


## 项目依赖
- github.com/dgrijalva/jwt-go v3.2.0+incompatible
- github.com/dgrijalva/jwt-go v3.2.0+incompatible
- github.com/gin-contrib/cors v1.4.0
- github.com/gin-gonic/gin v1.9.1
- github.com/go-playground/validator/v10 v10.14.0
- github.com/go-redis/redis/v8 v8.11.5
- github.com/google/uuid v1.1.2
- github.com/juju/ratelimit v1.0.2
- github.com/mojocn/base64Captcha v1.3.5
- github.com/mssola/useragent v1.0.0
- github.com/robfig/cron/v3 v3.0.1
- github.com/shirou/gopsutil v3.21.11+incompatible
- github.com/sirupsen/logrus v1.9.3
- github.com/spf13/viper v1.17.0
- github.com/tealeg/xlsx v1.0.5
- golang.org/x/crypto v0.14.0
- golang.org/x/net v0.15.0
- golang.org/x/text v0.14.0
- gorm.io/driver/mysql v1.5.2
- gorm.io/driver/postgres v1.5.4
- gorm.io/gorm v1.25.5

## 项目目录层级
* **api:** 存放后端 API 接口相关的代码
    * `common`: 通用部分
    * `init.go`: 初始化
    * `monitor`: 监控
    * `system`: 系统管理
* **cmd:** 存放可执行文件的主代码
    * `admin`: 管理后台
    * `job`: 定时任务
* **configs:** 存放配置相关文件
    * `embed.go`: 嵌入式配置
    * `release.yaml`: 发布版本配置
    * `test.yaml`: 测试版配置
* **data:** 存放数据文件
    * `ry_20230706.sql`: 示例数据库文件
* **internal:** 存放内部代码
    * `config`: 配置
    * `constant`: 常量
    * `db`: 数据库交互
    * `handler`: 处理器
    * `middleware`: 中间件
    * `model`: 模型
    * `response`: 响应
    * `router`: 路由
    * `service`: 服务
* **pkg:** 存放通用工具包
    * `captcha`: 验证码
    * `exceltool`: Excel 操作
    * `fileuploadtool`: 文件上传
    * `jwttool`: JWT 相关
    * `logger`: 日志
    * `redistool`: Redis 操作
    * `rsatool`: RSA 密码
    * `types`: 类型定义
    * `utils`: 实用工具
* **scripts:** 存放脚本文件
    * `build.sh`: 构建脚本
    * `deploy.sh`: 部署脚本
* **uploads:** 存放上传的文件
    * `blob_202402010947544c7300c145bd4c39b47146393a92a818.png`: 示例图片
    * `blob_202402010949583fa99fad65024ce9a4700866ef8bec15.png`: 示例图片
    * `blob_20240201101650459227b6007142699111a8474ec0bb3f.png`: 示例图片

## 优势
- 层级简单
- 最热门的框架选型
- java若依的的前端能直接套用
- 代码逻辑以及命名复刻率80%+
## 联系我请备注github
![我的二维码](img.png)
