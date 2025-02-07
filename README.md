# blog
个人博客

# hexo部署Pages流程

前提，github账号，ssh公钥已添加，电脑安装nodejs git，并且全局安装hexo

1. github 新建仓库，复制ssh地址，克隆到本地
2. IDE打开项目，初始化npm init -y
3. 新建src文件夹作为博客主文件夹，然后hexo init
4. 然后github仓库配置下
Settings->Pages->Source->Github Actions
Settings->Actions->General->Workflow permissions->Read and write permissions
5. 配置工作流和改url，
找到 deploy.yml  _config.yml 配置好对应的文件路径和最终访问地址
6. git push推送，然后自动部署，可以在github的Actions查看进度，完成后打开对应的地址即可