### git��github�Ĺ�ϵ

git��һ���汾�����ߣ�������ߣ���github����git���汾���Ƶ���Ŀ�й�ƽ̨��һ����վ����

### ��windows����ΰ�װGit��
   **msysgit**�� windows���Git,���£�
![](http://ww1.sinaimg.cn/mw690/6941baebgw1eloyr9g0xxj206u00tt8j.jpg)

#### ���°汾���ص�ַ
[���ص�ַ](https://git-for-windows.github.io/)

### ע��github�˺�
�ٷ���ַ��[https://github.com/](https://github.com/)
![](http://img.blog.csdn.net/20161215154849180?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvZmVuZ3Fpbmd0YW8yMDA4/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

ע�����   sign up ��ע�ᣬsign in �ǵ�¼
![](http://img.blog.csdn.net/20161219155249954?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvZmVuZ3Fpbmd0YW8yMDA4/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### �˽�һЩ��ϵͳ����

#### pwd 
��õ�ǰ����Ŀ¼

#### mkdir
����Ŀ¼�����ʽ����

> mkdir �½���Ŀ¼��
#### cd����
���뵽ĳ��Ŀ¼
> cd Ŀ¼��

������,���뵽d��helloĿ¼
```
cd d:/hello
```
### �˽ⳣ��git����

1. git��ʼ��

```
git init
```
������ִ�к�����һ��.git�������ļ��У�����ļ���������ǣ�

![image.png](http://upload-images.jianshu.io/upload_images/468490-cb8cde49aef4c341.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

����������ݣ��ᱣ�����Ƕ�����**��Ŀ**�������޸ĵļ�¼������ʹ�����ǻָ���֮ǰ���κ�״̬��

2. git add �ѹ��������ļ��ύ���ݴ���

git add �ļ���
git add . �����Ŀ¼�������ļ���

![](http://upload-images.jianshu.io/upload_images/1132519-c1ba4dea31c7c001.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)
3. git commit �ѹ��������ļ��ύ�����زֿ�Repository
git commit -m"�����ύ������"

��һ������git commit��������������ʾ��

![image.png](http://upload-images.jianshu.io/upload_images/468490-93d59782d2d28745.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

����취��
 1.�����û���
```
    git config --global user.name "zhangsan"
```
  2.�����û�������
```    
git config --global user.email  "zhangsan@sina.com"
```

### ���زֿ�����ܽ�

�½�һ����Ŀ�Ժ����ȵ���һ��git init�����ʼ��һ���ֿ⡣�����������ļ������Ӻ��޸ģ����� �ĵ���git add . ��git commit -m"xxx"��������������Ĺ��̱��浽�ֿ��С�

> ����Ϊֹ��github��û���κι�ϵ��

### �ѱ��زֿ�������ϴ���github

1. ��¼github����github�½�һ����Ӧ�Ĳֿ⣨�������ǵ���Ŀ��

2.������������ ��
git remote add Զ����Ŀ���� Զ����Ŀ��ַ
```
git remote add origin git@github.com:songboriceboy/my_novel_project.git
```
3. �����زֿ��ϴ�Զ�ֿ̲⣨github���Լ��û����½���Ŀ�У�

git push -u Զ�̵�ַ ���زֿ⣨Ĭ�Ͻ�master��

```
git push -u origin master
```
һ����Ҫ�����û��������룺��������ͼ��ʾ��
![image.png](http://upload-images.jianshu.io/upload_images/468490-7ef3aa80e6df7aae.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

��ʱ��������Ҫ���Լ��ĵ��ԣ���github�����Ϊ�����Ρ�

����SSH Key�����û���Ŀ¼�£�������û��.sshĿ¼������У��ٿ������Ŀ¼����û��id_rsa��id_rsa.pub�������ļ�������еĻ���ֱ������������������û�еĻ����������У������������

ssh-keygen  -t rsa �CC "zhangsan@sohu.com"