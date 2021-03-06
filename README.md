# AuditSQL审核执行平台

AuditSQL是web版本的MySQL数据库审核平台，旨在降低DBA的运维成本，谢谢。

使用上的问题，可以提ISSUES或者加QQ群。

## 组件
- Python 3.6
- Django 2.0
- AdminLTE 
  
## 功能
- 自定义工单环境
  - 可以根据公司业务需求，定义多个环境，比如：测试环境、预发布环境、生产环境等
- 工单类型
  - 支持DML、DDL、运维工单、数据导出工单(csv,xlsx)
  - 支持钩子、上线版本等功能
- 语法规则
  - 提供SQL语法审核、格式化、高亮、注释、补全等功能
- 审核流程
  - 流程化工单
  - 语法规则检测(目前inception仅做此用途)
  - 审核人审核工单，是否通过
  - 执行人执行工单，反馈工单状态
  - 工单历史
- 执行
  - DDL语句支持gh-ost改表
  - DML语句实现事务级别的执行保证
  - 支持一键「全部执行」和有选择的「单条执行」
  - 自动生成DML备份语句 
- 进度展示
  - 前台实时显示DML、DDL、数据导出的进度（websocket）
- 推送通知
  - 支持钉钉机器人
  - 支持邮件推送
  - all
- SQL查询
  - MySQL查询功能
  - 支持表级授权
  - 通过规则链和规则组实现灵活的授权
  - 支持查看表结构、索引、元信息，支持补全、格式、limit等功能
- Xterm
  - 支持Xterm接口，提供更丰富的扩展功能，可以接入redis、mongodb等命令行接口，实现查询
- 数据导出
  - 支持xlsx，csv格式，支持海量数据的优化导出
- 其他功能
   - 支持自定义角色
   - 支持LDAP授权登陆功能
   - 支持本地自建用户，本地密码修改
   - 支持修改头像


## 效果展示
https://github.com/lazzyfu/AuditSQL/wiki/show

## 文档（使用和安装）
https://github.com/lazzyfu/AuditSQL/wiki

## 联系方式：
QQ群号：710797678

欢迎大家贡献代码，感谢大家的支持，谢谢

## 感谢
@HaroldZhen 贡献代码

