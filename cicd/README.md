> 准备工作
  1. 文件挂载路径
  ```
  export GITLAB_HOME="/Users/michael/gitlab"
  ```

> 运行/更新
  ```
  docker compose up -d
  ```

> login
  1. first time

  - gitlab
    - address: https://localhost/user/sign_in
    - user: root
    - password: cat /etc/gitlab/initial_root_password
                w152****
  - jenkins
      - install plugins
      - new user
        - user： admin
        - password： admin123

    ```
    使用 root 用户登陆jenkins
    docker ps
    docker start [containerId]
    docker exec -it -u root [containerId] sh
    ```
    > 遇到的问题及解决方案
    <br>
    教程：https://www.cnblogs.com/SmilingEye/p/11429827.html <br>
    root 权限问题： https://blog.csdn.net/liumiaocn/article/details/102634568 <br>
    debian 系统 install nodejs： https://www.xtuos.com/3472.html <br>
    同步时区 https://blog.csdn.net/qq_34885615/article/details/109536384 <br>
    无法执行source： https://blog.csdn.net/miracle_zero/article/details/122809546


    后记：
    关于 nvm nodejs 可使用 nvm-wrapper 不用辛苦哈哈的去破解 root