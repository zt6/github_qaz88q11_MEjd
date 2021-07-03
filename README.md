######V4更换默认LXK地址###########
1、进容器 (XXX为自己容器名)：docker exec -it XXX bash
2、编辑jup：vi jup.sh
3、按 i 编辑，然后通过键盘的上下左右箭头来定位。
4、第6行改为要替换的主库地址，如：url_scripts=https://github.com/Annyoo2021/scripts.git
5、第454行 若仓库分支不同，需更改分支，如lxk的master改成新库的main：git_clone_scripts $url_scripts $dir_scripts "main"
6、第429行注释：#random_update_jup_cron
     这一行为 更新jup任务的随机定时，注释掉便可自定义jup更新的定时，而保持不变了。
7、第598行取消注释：update_scripts
8、按esc退出编辑，然后输入:wq!  再回车 (此处为小写冒号，一并输入)
