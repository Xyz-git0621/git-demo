项目简介 
本项目是基于 JavaFX 开发的桌面应用项目，实现对应业务功能。
本仓库仅存放项目源代码，部分外部素材资源未纳入版本管理，需要开发者本地自行配置。


环境依赖
- JDK 17（支持JavaFX）
- 项目内置Maven Wrapper，无需本地额外安装Maven


克隆仓库完成后，部分外部素材需要手动放置到对应路径：

plaintext
src/main/resources/assets/thegame/images
 images 目录已加入gitignore，不会提交到版本库；项目原创资源放置于 assets/thegame/original_images ，跟随仓库同步。

 
 images 目录已加入gitignore，不会提交到版本库；项目原创资源放置于 assets/thegame/original_images ，跟随仓库同步。


编译运行
Windows PowerShell终端执行：

shell
# 编译项目
./mvnw.cmd compile

# 启动JavaFX应用
./mvnw.cmd javafx:run
角色与分工
孙嘉轩 组长PM 敲定分工与架构内容
肖雨泽 开发 JavaFX主界面、页面布局、事件交互 
黄磊 开发 业务逻辑、数据模型、工具类编写 
赵嘉良 开发 配置管理、文件读写、素材处理 
王宇坤 测试/文档 功能测试、bug修复、维护项目文档  
王宇坤 测试/文档 功能测试、bug修复、维护项目文档 

分工计划
1. 前期：搭建JavaFX项目骨架，统一Maven依赖、Git团队协作规范，完成目录结构、 .gitignore 、README文档，统一全体成员开发环境。
2. 中期：拆分模块并行开发，每个人在独立功能分支完成各自模块；开发完成后提交PR合并至 dev 开发分支；定期联调，解决界面与业务逻辑对接问题。
3. 后期：整体测试修复bug，整合全部功能，合并至 master 稳定分支，完成最终版本打包。
Git规范： master 为最终稳定版本，禁止直接push；新功能从 dev 分支切出 feat/xxx 分支开发。

AI使用与核对说明
1. 开发过程中使用AI工具用于：代码思路参考、JavaFX语法查询、生成工具代码、文档撰写、报错排查。
2. 所有AI生成代码均经过组员人工阅读、核对、修改调试，确认逻辑正确后才纳入项目。