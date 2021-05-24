# 邓永盛的机器人后台数据
邓永盛的机器人数据库后台数据导出，sqlserver格式  
  
下载后直接附加到sqlserver数据库即可，注意添加时无ldf文件  

# 表目录  

| Tables_in_小one易健康打卡        |
| --------   |
| 令牌表        |
| 打卡完成记录        |
| 统计                      |
| 错误日志                  |

+---------------------------+
| Tables_in_小one易健康打卡 |
+---------------------------+
| 令牌表                    |
| 打卡完成记录              |
| 消息发送日志              |
| 班级表                    |
| 统计                      |
| 错误日志                  |
+---------------------------+

# 注意
这里的手机号码和班群群号都上传之前被修改过，并非物理世界的真实信息  

# 主要操作：
1.根据`班级表`和`令牌表`来查询班级和最 对应班级管理员的最新的一条token信息，qq群号，qq群名，班级名，学院名  
  
2.根据`班级表`和`打卡完成记录`来查询某一天未完成打卡的班级  
  
3.根据`班级表`中的班级id，和一条新的管理员token 插入到`令牌表`  
  
4.根据`消息发送日志`来统计汇总已经累计提醒了的人次和消息发送的提醒信息条数，即`统计`视图  
  
5.根据 `班级表`和`消息发送日志`来统计各班每天的打卡完成时间
