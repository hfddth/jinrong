# DeepSeek 安全后端

Node.js 22+，无需依赖。把此目录部署到支持Node长期服务的主机（不要使用GitHub Pages执行后端）。启动命令 `npm start`。通过主机Secret/Environment设置 .env.example 列出的变量；程序不自动加载.env文件。

必须使用重新生成的DEEPSEEK_API_KEY，切勿提交真实密钥。deepseek-flash是官方DeepSeek V4.1 Flash API标识。仅使用官方 https://api.deepseek.com 服务。

配置HTTPS域名后，在评估页输入该域名以及独立的FTIOR_ACCESS_TOKEN访问口令。不要在网页中输入DeepSeek密钥。访问口令适用于私有试用；公网运营前需接入账号认证、用户级配额与可靠限流。本版同一实例只允许一个并行任务。

前端仅在明确勾选同意后发送已解析全文，最长18万字符，超限直接拒绝，不静默截断。服务器不保存正文、不记录密钥或请求正文。模型输出须通过五维字段和原文引用验证；缺失证据的分数置空，综合分及等级待评估，额度保持空值。模型建议始终为草稿，专业人员复核后才能采用。

未配置环境变量时接口返回503，绝不以演示结果冒充真实调用。
