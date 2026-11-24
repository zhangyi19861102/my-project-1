# 软件新版本发布仓

本仓库只存放软件安装包与版本清单，供 NSPack 生成的在线安装包自动下载。

## 固定下载地址（每次发版都会指向最新版本）

- 版本清单：https://github.com/zhangyi19861102/my-project-1/releases/latest/download/latest.json
- 扁平清单：https://github.com/zhangyi19861102/my-project-1/releases/latest/download/latest.txt
- 安装包：https://github.com/zhangyi19861102/my-project-1/releases/latest/download/<安装包文件名>

## 发版步骤

1. NSPack 点「开始构建」，输出目录会得到离线包、在线包、latest.json、latest.txt
2. 打 tag 并上传资产（gh release create v<版本> 输出\*）
3. 客户端下次运行在线安装包会自动读到最新版本
