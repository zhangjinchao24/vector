vector

string头文件
#include <string>
  using std::string;
  
初始化:
  string s1;
  string s2(s1);
  string s2=s1;
  string s3（“value”）;
  string s3="value";
  string s4(n,'c')
  
string与字符或字符串字面值相加时应保证+两侧至少有一个为string
  string s2="hello"+s1+'\n';
  string s3="hello"+'\n'+s1;//错误

基于范围的for语句(不仅仅是适用于string类型)
  for(auto &c:s)    //c定义为引用时可通过c改变对象s中的值
  c='h';
  
  
 
 插入、删除、、复制、查找、比较

相关函数

赋值

阅读：循环、switch使用

好的程序需要考虑
正确性：遇到错误输入直接结束，返回输入错误警告
健壮性：对非法输入进行分析，尝试将其转换为合法输入     //chagnshi尝试
可靠性
稳定性
可读性
高效性
简洁性

编程习惯
变量名称
换行符
括号:可以略去括号的时候省略，但要注意换行


问题
字符或字符串字面值是否能直接 相加
如何实现将以下两个判断合并到一处且不影响执行顺序？
  if(a==0)
    int step1;
  int step2;
  if(a==0)
    int step3;
    
  常见错误
   无返回值
   判断时=和==
