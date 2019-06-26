## 								linux常用命令

* 卸载 Ubuntu 自带的 openjdk 的方法：

  执行命令：***sudo apt-get remove openjdk\****  

  ------

* 修改权限的命令

  执行命令: chmod 777 文件名

  ***

* **tomcat 服务相关**

  * 启动/关闭tomcat服务

    sudo ./startup.sh    sudo ./shutdown.sh

    

    查看日志:

    tail -f catalina.out
  
    Linux系统中使用以下命令来查看文件的内容：
  
    - cat  由第一行开始显示文件内容
    - tac  从最后一行开始显示，可以看出 tac 是 cat 的倒著写！
    - nl   显示的时候，顺道输出行号！
    - more 一页一页的显示文件内容
    - less 与 more 类似，但是比 more 更好的是，他可以往前翻页！
    - head 只看头几行
    - tail 只看尾巴几行
  
    
  
  * 配置tomcat相关系统环境变量
  
    编辑bin目录 下的startup.sh文件 , 在最下面加上
  
    ```
    export TOMCAT_HOME=/usr/local/apache-tomcat-8.5.31
    ```

***

*   **mysql相关知识**

  重启数据库服务
  
  ```
  service mysql restart;
  ```
  
  ------
  
  添加普通索引:
  
  ```
  ALTER TABLE table ADD INDEX birthday_index (birthday);
  ```
  
  查看表中所有索引:
  
  ```
  show  index from table(表名);
  ```
  
  删除索引:
  
  ```
  drop index idx_xxx on table(表名);
  ```
  
  