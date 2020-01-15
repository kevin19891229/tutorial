> 注意：
> 1. docker image build 和 docker build功能相同
> 2. 如果是root, 可以不使用sudo

# docker image的构建过程
1. 将自己的代码放置src目录
2. 编写Dockerfile：菜鸟教程：https://www.runoob.com/docker/docker-dockerfile.html
3. sudo docker build . -t yb19891229/test-dockerfile
4. 查看已经生成的image: sudo docker images
5. 试运行：sudo docker run yb19891229/test-dockerfile
6. 查看docker运行状态：sudo docker ps -a
7. 发布到docker hub：
   1. 在hub.docker.com注册帐号(不同公司会搭建自己的docker hub)
   2. 登录：sudo docker login
   3. 发布：sudo docker push yb19891229/test-dockerfile:latest
   4. 去docker hub查看上传情况：https://hub.docker.com/repository/docker/yb19891229/test-dockerfile
