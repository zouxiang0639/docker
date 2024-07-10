# docker
## es es-docker-compose.yml
### 启动命令
~~~
docker-compose -f es-docker-compose.yml down
docker-compose -f es-docker-compose.yml up --build -d
~~~

### http://localhost:5601/app/dev_tools#/console
~~~
POST /_analyze
{
"analyzer": "ik_max_word",
"text": "这是一个包含自定义词1和停用词1的测试"
}

## mysql mysql-docker-compose.yml
### 启动命令
~~~
docker-compose -f mysql-docker-compose.yml down
docker-compose -f mysql-docker-compose.yml up --build -d
~~~



## consul consul-docker-compose.yml
~~~
docker-compose -f consul-docker-compose.yml down
docker-compose -f consul-docker-compose.yml up --build -d
~~~

### http://localhost:8500/ui/dc1/acls/tokens
~~~
AccessorID:       f645c42e-8b59-d000-0977-8aa6004ecc90
SecretID:         ae869790-92e4-02c3-d64a-7d50123b383a
Description:      Bootstrap Token (Global Management)
Local:            false
Create Time:      2024-06-26 02:09:12.764177837 +0000 UTC
Policies:
   00000000-0000-0000-0000-000000000001 - global-management
   

   
只能查看权限
a685040a-7dfa-1da9-a2fc-88d4cadedbac