# go-qwen

由于阿里百炼平台通义千问大模型没有完善的go语言示例，并且官方答复assistant是不兼容openapi sdk的。
实际使用中发现是能够支持的，所以自己写了一个demo test示例，给大家做一个参考。

# apikey 生成官方教程
https://help.aliyun.com/zh/model-studio/getting-started/first-api-call-to-qwen

## ✨ 说明
- utils 中写的是获取实例的方式
- const 中写的是baseUrl 具体的千问访问url，以及调用时候用到的apiKey （需要自己申请 sk-xxxx 格式）
- -----------------------------------------------------------------------------------------------------------------
- full_step_test 完整流程
- chat_test 普通的聊天示例
- chat_stream_test 普通的聊天示例-流式输出
- assistant_test 助手增删改查
- tread_test 会话示例
- message_test 消息示例
- run_test 运行任务示例
- -----------------------------------------------------------------------------------------------------------------
## ✨ assistant 流程
    1. 创建助手 
    2. 创建会话
    3. 创建消息(在会话上创建)
    4. 创建执行任务（执行会话）
    5. 获取最后一次执行结果
