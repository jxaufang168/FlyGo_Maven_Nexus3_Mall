# FlyGo_Maven_Nexus3_Mall
FlyGo_Maven_Nexus3_Mall

文档地址：https://www.flygo520.com/docs/maven/maven-1an1jq32d71ge

修改工程中的 `pom.xml` 配置文件，填写你的私服地址。

```bash
<distributionManagement>
  <repository>
    <!-- 对应Maven setting.xml配置文件中 server 一一对应 -->
    <id>mall-releases</id>
    <name>Mall Release Repository</name>
    <url>http://${你的私服地址}/repository/mall-releases/</url>
  </repository>
  <snapshotRepository>
    <!-- 对应Maven setting.xml配置文件中 server 一一对应 -->
    <id>mall-snapshots</id>
    <name>Mall snapshot Repository</name>
    <url>http://${你的私服地址}/repository/mall-snapshots/</url>
    </snapshotRepository>
</distributionManagement>
