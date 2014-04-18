#spring-oauth-server


<strong>Spring与Oauth2的整合示例</strong>

项目用Maven管理


使用的技术与版本号
<ol>
 <li>Spring (3.1.1.RELEASE)</li>
 <li>Spring Security (3.1.0.RELEASE)</li>
 <li>MyBatis (3.2.1)</li>
 <li>spring-security-oauth2 (1.0.5.RELEASE)</li>
</ol>


<p>
<strong>如何使用?</strong>
1.项目是Maven管理的, 需要本地安装maven(开发用的maven版本号为3.1.0), 还有MySql(开发用的mysql版本号为5.5)

2.下载(或clone)项目到本地

3.创建MySQL数据库(如数据库名oauth2), 并运行相应的SQL脚本(脚本文件位于others/database目录),
   运行脚本的顺序: initial_db.ddl -> oauth.ddl -> initial_data.ddl

4.修改spring-oauth-server.properties(位于src/resources目录)中的数据库连接信息(包括username, password等)

5.将本地项目导入到IDE(如Intellij IDEA)中,配置Tomcat(或类似的servelt运行服务器), 并启动Tomcat(默认端口为8080)
   另: 也可通过maven package命令将项目编译为war文件(spring-oauth-server.war),
         将war放在Tomcat中并启动(注意: 这种方式需要将spring-oauth-server.properties加入到classpath中并正确配置数据库连接信息).

6.参考oauth_test.txt(位于others目录)的内容并测试之(也可在浏览器中访问相应的地址,如: http://localhost:8080/spring-oauth-server).

</p>

<hr/>

<p>
 与该项目相关的博客请访问 <a target="_blank" href="http://blog.csdn.net/monkeyking1987/article/details/16828059">http://blog.csdn.net/monkeyking1987/article/details/16828059</a>
</p>


<p>
 欢迎发邮件到<a href="mailto:monkeyk1987@gmail.com">monkeyk1987@gmail.com</a>一起讨论.
</p>