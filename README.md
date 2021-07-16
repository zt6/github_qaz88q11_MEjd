
镜像默认用我的库作为主库，三方库自行添加。装好更新后，安装某些脚本所需依赖：

（依次执行以下命令，默认容器名jd_v4_bot，如做了修改，按实际修改命令。）

docker exec -it jd_v4_bot bash

cd scripts && npm install png-js
