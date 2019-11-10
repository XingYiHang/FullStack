### 样式b表位置
- 内联样式（耦合度大，不利维护，不推荐使用）例：<P style="color:red; font-size:40px;"></p>
- 写到<style></style>标签中(初步分离)
```
<!DOCTYPE HTML>
<html>
      <head>
            <meta charset="UTF-8">
            <title>标题</title>
            <!-- -->
            <style type="text/css">
                    <!--标签选择器-->
                    p{
                      color:red;
                      font-size:20px;
                      }
            </style>
      </head>
      <body>
            <p>内容</p>
      </body>
</html>
```
-外联式 <link rel="stylesheet" type="text/css" href="">（完全分离，易于复用，）
