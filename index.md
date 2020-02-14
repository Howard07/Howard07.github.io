## 新年快乐2020
----
# Welcome to Howard07 #
---
<blockquote>混一天和努力一天，一天看不出任何差别，三天看不到任何变化，七天也看不到任何距离……但是一个月后会看到话题不同，三个月后会看到气场不同，半年后会看到距离不同，一年后会看到人生道路截然不同。<br>
2019年的冬天不是靠熬能够过去的。任正非<br>
-==每一件与众不同的绝世好东西，都是以无比的勤奋为前提。要么是血，要么是汗，要么是大把大把的曼妙好时光。==让我们一起迎接即将到来的2020!吴晓波</blockquote>



#c\c++
1.[对argc与argv的认识](https://blog.csdn.net/u014106566/article/details/84141718)
>C/C++语言中的main函数，经常带有参数argc，argv，如下：int main(int argc, char ****argv)或int main(int argc, char * argv[])
main (argc,char * argv[]){while(- -argc>0)printf("%s",argv[argc]);printf("\n");}
<br>第一个int argc，是argument count的缩写，表示传入main函数的参数个数,记录你输入在命令行上的字符串（参数）个数；第二个 * argv[]是argument vector的缩写,表示传入main函数的参数序列或指针，存放输入在命令行上的命令（字符串）。当命令行输入PROG ABCDEFGH  IJKL时，记录了3个字符串（以间隔为界，不含间隔，这是约定），* argv[0]中放的是"PROG"，* argv[1]中放的是"ABCDEFGH"，* argv[2]中放的是"IJKL"，这样argc就是3了。while(--argc>0)是条件循环，argc>0时继续；argc初值是3，前置--先减1为2，所以后面的输出语句打出* argv[2]中的内容IJKL；再执行while(--argc>0)，argc再减1为1，打出* argv[1]中的内容ABCDEFGH；再循环，argc减1为0，条件破坏，不再执行while(--argc>0)的循环体。所以最后显示的是IJKLABCDEFGH。

---
2.[C语言strcat 函数-字符串连接函数](https://www.shiyanlou.com/courses/57/learning/?id=357)
-需要用到的头文件#include<string.h>
<blockquote>int main(){
   char str1[30] = "People's Republic of'";
   char str2[] = "China";

   printf("%s",strcat(str1,str2));
   return 0;}#include<iostream>
#include<cmath>
#include<iomanip>
using namespace std;
int main(){
	float r,x,p,y;
	cin>>r>>x>>p;
	y=x*pow(((100+r)/100),p);
	cout<<fixed<<setprecision(2)<<y<<endl;
	return 0;
}
  <br> 输出结果：People's Republic of'China
</blockquote>

3.输出答案x，结果保留2位数
>头文件'#include<iomanip>'
''cout<<fixed<<setprecision(2)<<x<<endl;''


