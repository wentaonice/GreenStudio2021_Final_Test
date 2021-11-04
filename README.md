# 绿荫工作室2021年招新最终审核

### 请在本目录下或者本文件下提交项目代码/截图:

计1907李牧霖: 我在等着我的小学弟/学妹们提交文件~
[新建 Microsoft Word 文档.docx](https://github.com/Mr-Lobster/GreenStudio2021_Final_Test/files/7473163/Microsoft.Word.docx)
![未来的计划与期望](https://user-images.githubusercontent.com/93137540/140278449-f30759c9-bd72-46e9-9748-dcd31202db24.PNG)
#include <iostream>
using namespace std;

int main()
{
	cout << "希望能够在大学中加入和编程有关的团体或者组织，来提升自己的能力"<<endl;
	cout << "多参加竞赛，第一个让自己开阔眼界，第二个让自己有资本与他人竞争"<<endl;
	cout << "学习新知识的同时，能够去实践来融会贯通并为社会做一些贡献"<<endl;
	cout << "在大学多拿奖学金，这是我的目标"<<endl;
	cout << "能够找到三五个志同道合的伙伴，一起向目标进发，也是我的希望"<<endl;
}


  
//设计一个程序，要求对一个不大于5位的正整数能：
//（1）判断出它是几位数；
//（2）求其逆序数并输出。
#include<iostream>
using namespace std;

int main()
{
	int number = 0, i = 0, c, d;//i用于计数，赋予number值为零
	cout << "请输入一位不大于五位的整数";
	cin >> number;
	d = number;//之后要让输入的数逆位输出，但之前判断是几位数时已经让number为零了，故将其存储到d中
	while (number > 0)
	{
		number = number / 10;//整数除整数还为整数，一直除到零，除了几次，就为几位数
		i++;
	}
	cout << "这是" << i << "位数" << endl;
	while (d > 0)
	{
		c = d % 10;//将最右边的数剔出来并输出
		cout << c;
		d = d / 10;//将最右边的数去掉
	}
