# 学习进度
## 2026-10-23
1、 curl 验证请求，大模型调用，如下windows环境，cmd调用验证：

curl -X POST https://dashscope.aliyuncs.com/compatible-mode/v1/chat/completions -H "Content-Type: application/json" -H "Authorization: Bearer sk-ws-H.PERHDIE.zzFO.MEQCIFE0iTeSwEE7o18nXVxDoGKD2CgSirzsgg1yEI7cdf_aAiBIGF0F6-3ojSf8bGHOfmhjFOoH8Jdjm3T8IwuYeuMi-A" -d "{\"model\":\"qwen-plus\",\"messages\":[{\"role\":\"user\",\"content\":\"你好\"}],\"max_tokens\":50}"

- cmd输出这个表示调用成功
{"model":"qwen-plus","id":"chatcmpl-c999cafd-a4cb-9972-999b-42c0bafa4983","choices":[{"message":{"content":"你好！很高兴见到你～😊 有什么我可以帮你的吗？无论是学习、工作、生活中的问题，还是想聊聊天、获取信息、一起动脑筋，我都很乐意帮忙！","role":"assistant"},"index":0,"finish_reason":"stop"}],"created":1792744460,"object":"chat.completion","usage":{"total_tokens":50,"completion_tokens":41,"prompt_tokens":9,"prompt_tokens_details":{"cached_tokens":0}}}