[TOC]
jobconverter镜像

# 适用场景
适用于开发测试环境

# 功能
## office文件转换为pdf,html,txt,xhtml png,docx,rtf,sxw,odt等格式文件



# 使用方式
```
# 构建
# docker build -t qq275860560/jobconverter .
# 拉取
docker pull qq275860560/jobconverter
# 运行
docker run -d -p 8080:8080 qq275860560/jobconverter 
# 测试
存在c:/test.docx,希望转换为pdf文件，把结果存储为c:/result.pdf
curl -o c:/result.pdf  -X POST 'http://localhost:8080/lool/convert-to' -F 'data=@C:/test.docx;type=application/octet-stream' -F 'format=pdf'
```
 

# 温馨提醒

* 此项目将会长期维护，增加或改进实用的功能
* 右上角点击star，给我继续前进的动力,谢谢