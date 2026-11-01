# 银智养融官网与资料复核平台 v2

主入口 index.html；上传解析 assessment.html；人工专业复核 expert-review.html。

支持DOCX、UTF-8 TXT/CSV/JSON本地解析。DOCX使用浏览器DecompressionStream，浏览器不支持时明确失败；PDF与扫描件需要转换或OCR。关键词仅建立候选证据索引，不自动评分。无后端、无文件外传、无大模型API。

待复核报告包含文件状态、来源段落、五维缺口和待办；人工评分后沿用FTIOR固定权重生成辅助报告。案例在独立cases.html，不参与真实企业评分。
