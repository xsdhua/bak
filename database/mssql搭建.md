



微软提供了9个内置的角色，以便于在数据库级别授予用户特殊的权限集合

db_owner:该角色的用户可以在数据库中执行任何操作。
db_accessadmin:该角色的成员可以从数据库中增加或者删除用户。
db_backupopperator:该角色的成员允许备份数据库。
db_datareader:该角色的成员允许从任何表读取任何数据。
db_datawriter:该角色的成员允许往任何表写入数据。
db_ddladmin：该角色的成员允许在数据库中增加、修改或者删除任何对象（即可以执行任何DDL语句）。
db_denydatareader:该角色的成员被拒绝查看数据库中的任何数据，但是他们仍然可以通过存储过程来查看。
db_denydatawriter: 像db_denydatareader角色，该角色的成员被拒绝修改数据库中的任何数据，但是他们仍然可以通过存储过程来修改。
db_securityadmin:该角色的成员可以更改数据库中的权限和角色。
public：在SQL Server 2008中每个数据库用户都属于public数据库角色。当尚未对某个用户授予或者拒绝对安全对象的特定权限时，这该用户将据称授予该安全对象的public角色的权限，这个数据库角色不能被删除

sa是默认超级管理员

脚本运行
osql help

osql -Usa -PXsd123$ -i "file"

-S 服务器ip 
-d 数据库名称
-U 连接用户名
-P 用户的密码
-i 执行的sql文件
-o sql语句输出的结果文件