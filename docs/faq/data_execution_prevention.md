# 正常关闭数据执行保护

## 右击计算机，选择属性

![dep-1.png](img/dep-1.png)

## 选择高级系统设置

![dep-2.png](img/dep-2.png)

## 点击高级，选择设置

![dep-3.png](img/dep-3.png)

## 选择数据执行保护，然后在下面仅为基本windows程序和服务启用DEP前面点亮，然后点击确定

![dep-4.png](img/dep-4.png)

# 数据执行保护呈灰色时关闭

:::caution
默认的管理员账号是关闭开不了的
需要创建一个新的管理员账户才能关闭
:::

## 创建一个新管理员账户

### 进入控制面板

![dep-5.png](img/dep-5.png)

### 在大图标下进入用户账户

![dep-6.png](img/dep-6.png)

### 在电脑设置中添加新用户

![dep-7.png](img/dep-7.png)

### 管理其他账户

![dep-8.png](img/dep-8.png)

### 添加账户

![dep-9.png](img/dep-9.png)

### 输入你要创建的这个账户的一些信息

![dep-10.png](img/dep-10.png)

:::caution
记得要管理员权限
:::

## 登陆新创的账户

:::info
只要注销在登录的时候切换成新账户就行了（由于我的电脑不需要，所以没截图了）
:::

## 输入指令

### 在开始页输入cmd并以管理员身份运行

![dep-11.png](img/dep-11.png)

### 输入 `bcdedit /set nx optin alwaysoff` 并回车运行后重启

![dep-12.png](img/dep-12.png)

## 再切换回你之前的账户

你就看到你成功啦，你会发现，DEP也被开启了