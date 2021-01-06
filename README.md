# 6hao

#大一上python的代码 
##猜数游戏   
```  

```
##斐波那契数列
```
M=int(input())
def f_(a):
    if a == 2:
        return 1
    elif a == 3:
        return 2
    elif a == 4:
        return 4
    return f_(a-1)+f_(a-2)+f_(a-3)
print(f_(M))  
```
```
a=int(input())
def f_(b):       #递归函数
    if b==1:
        return 1
    elif b == 2:
        return 2
    elif b== 3:
        return 6
    return b*f_(b-1)    #n的阶乘
f_(a)
c=list(str(f_(a)))
c.reverse()
for score in c:
    if score !='0':   
       print(score)
       break  
```
##排序  
##九九乘法表  
```
for i in range(1,10):  #一共有十行
    for a in range (1,i+1):
        b = a*i
        print("%d*%d=%d"%(a,i,b),end=" ")    #以空格隔开
    print()         #一次for循环完后，换行
```
##自测题  

```
print("欢迎使用算术自测程序，测试开始：")
a=[]
b=[]
c=[]
import random
for i in range(1,11):
  d=random.randint(1,10)
  e=random.choice('+''-''*''/')
  f=random.randint(1,10)
  g=("第%d题：%d%s%d="%(i,d,e,f))
  if e=='+':
      h=d+f
      c.append(h)
  elif e=='-':
      h=d-f
      c.append(h)
  elif e=='*':
      h=d*f
      c.append(h)
  elif e=='/':
      h=d/f
      c.append(h)
  a.append(g)
  print(g,end=" ")
  k=int(input())
  #
  b.append(k)
print("测试结束")
for m in range(10):
    if b[m]==c[m]:
        print(a[m],b[m],  "√")
    else:
        print(a[m],b[m],  "×", c[m])  

```
### format 的用法：    
#### 0,1格式化输出  
```  
print('{0}'在'{1}'.format('我','玩游戏'))    #我在玩游戏  
print('{1}'在'{0}'.format('我','玩游戏'))    #玩游戏在我  
print('{1}'在'{1}'.format('我','玩游戏'))    #玩游戏在玩游戏   
```
#### b,o,d,h  分别代表二 八 十 十六 进制  
```  
#从小到大输出0-32的五位二进制数    
for i in range(5)  
print('{:05b}'.format(i))  
```
![](D:\信息素养作业图片/图.jpg)
#### format控制间距  
```  
#< ^ > 代表靠左 居中 靠右   10：字段长度（最左到最右之间的长度)  
print('{:>80}'.format('wo'))    #从最左到最右80时的最靠右边
print('{:>30}'.format('wo'))    #从最左到最右80时的最靠右边
print('{:^80}'.format('wo'))    #从最左到最右80时的居中
print('{:^30}'.format('wo'))    #从最左到最右30时的居中
```
![](D:\信息素养作业图片/tu.jpg)
#### format 小数点后几位 四舍五入  或  补0  
```    
print('{:.3f}'.format(1.34159))    #1.342
print('{:.5f}'.format(1.34))       #1.34000
 
```
#### chr  65表示A 以此类推  
![](D:\信息素养作业图片/3.jpg)    
```  
n=int(input())
word=65  
a='
for i in range(n)
	a=a+chr(word)+a 
    word += 1  
print(a)  
```
#### n的阶乘  
```  
n=int(input())
def f_(a):
    if a==1:
        return 1
    elif a==2:
        return 2
    elif  a>2:
        return a*f_(a-1)
print(f_(n))  
```


