﻿# cdrf  
Csharp Database Persistence Framework  
## cdrf是什么？  
cdrf是一个数据持久化框架，该框架就是为了实现将内存中的对象模型转换为存储模型。即将指定的对象转化为SQL语句并且对数据库进行增删改查等操作。  
## cdrf如何使用？  
1.在运行目录下创建一个xml文件并配置，调用Sql.init加载配置文件
2.调用Sql类下的函数实现增删改查等功能。函数的参数是任意的对象，但是必须保证类名与数据库中的表名相同，并且所在的命名空间已在配置文件中注册过。  
3.Sql.getInstance()可以获得Sql类的唯一对象
## cdrf有什么特点？
该框架的特点就是简单易于使用，相比其他的数据持久化框架，它不需要配置一堆复杂的xml文件，只需要保持类中的所有名字与数据库中表的名字都相同即可。但是也因为这一点，该框架的灵活性与可拓展性不如其他的框架。不过对于刚刚入门的开发者来说一个源代码不长且易于使用的开源数据持久化框架能够大幅减少开发的难度与所需的时间。
