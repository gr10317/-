
#include<stdlib.h>
#include<stdio.h>
#include<cstdlib>
#include <conio.h>   //包含数据输入输出函数，密码以不回显方式输入函数（getch();）的头文件
#include<iostream>
using namespace std;
#include<string.h>
//void cinn();//预防输入字符
//病人类
class Patient
{
public:
    Patient();//默认构造函数
    Patient(char Name[],char i[],int a,int n,int q);//一般构造函数
    ~Patient(){}
    void Input();//输入函数
    void Output();//显示函数
    int getNum();//返回序列号
    int getQue();//返回病人优先级
	void cinn1()
	{
		cinn();
	};//预防输入字符
private:
    char name[20];//姓名
    char ill[50];//病情
    int age;//年龄
    int num;//序列号
    int que;//优先级
	void cinn()
{
	//int age;
	while(!scanf("%d",&age))
{
	fflush(stdin);
	cout<<"请重新输入：";
}
}
};
//void cinn()
//{
//	int age;
//	while(!scanf("%d",&age))
//{
//	fflush(stdin);
//	cout<<"请重新输入：";
//}
//}


#define Num 2000 //排队号码将以2000后开始
static int lists=0; //普通挂号的人员
static int treat=0; //急诊挂号的人员
//默认构造函数
Patient::Patient()
{
strcpy_s(name," ");
strcpy_s(ill," ");
age = 0;
num = 0;
que = 0;
}
//一般构造函数
Patient::Patient(char Name[],char i[],int a,int n,int q):age(a),num(n),que(q)
{
strcpy_s(name,Name);
strcpy_s(ill,i);
}
//输入函数
void chi()
{
	char c;
	while((c=getchar())!='\n');
	return;
}
void Patient::Input()
{
printf("\t  姓名:");
cin>>name;
printf("\t  症状：");
cin>>ill;
printf("\t  年龄：");
cinn();
printf("\t  优先级(高为1，低为0)：");
cinn();
//cin>>age;
if(que == 0)
{
num = Num + (++lists);
printf("\n\t+———-挂号成功,您的排队号码为:———+\n\n %d\n\n",num);
printf("\t+————-您当前的位置为：%d————-+\n",lists+treat);
printf("\n\t+———友情提示：当有急诊病人挂号时候—–+\n");
printf("\t+———-此系统将以急诊病人的挂号优先——+\n");
printf("\t+————您排队的位置可能会有改变——–+\n\n");
}
if(que == 1)
{
num = Num + (++treat) -1000;
printf("\n\t+———-挂号成功,您的排队号码为:———+\n\n %d\n\n",num);
printf("\t+————-您当前的位置为：%d————-+\n",treat);

}
}
//输出函数
void Patient::Output()
{
printf("\t  姓名：%s\n",name);
printf("\t  症状：%s\n",ill);
printf("\t  年龄：%d\n",age);
printf("\t  排队编号：%d\n",num);
if(que == 1)
printf("\t  优先级：高\n");
if(que == 0)
printf("\t  优先级：低\n");
}
//返回病人优先级
int Patient::getQue()
{
return que;
}
//返回序列号
int Patient::getNum()
{
return num;
}

/*链表结点，即队列中的元素*/
typedef Patient ElemType;
typedef struct Node
{
    ElemType data;        //队列中元素的值
    Node* next;  //链表节点指针
}QNode,PNode;//定义普通病人和急诊病人对象

/*基于链表的队列的类*/
class LinkQueue
{
public:
    LinkQueue();
    ~LinkQueue();
    ElemType front();//获取头元素
    void Input();//输入函数
    void Output(ElemType e);//输出函数
    bool pop1();   //普通病人出队
    bool pop2();   //急诊病人出队
    bool Ordinary(ElemType e); //普通病人入队
    bool Emergency(ElemType e); //急诊病人入队
    void enroll();//医护人员登录系统
    void Doctor();//医生就诊系统
    bool isEmpty1();     //判空
	bool isEmpty2();     //判空
    int size();         //队列的大小
private:
    QNode * head ; //头指针
    QNode * tail; //尾指针
    PNode * h;//头指针
    PNode * t;//尾指针
    int len;    //队列长度
    int lists;//普通病人个数
    int treat;//急诊病人个数
};

static int success = 0;  //账户密码是否成功登陆
//构造函数
LinkQueue::LinkQueue()
{
    head = NULL;
    tail = NULL; 
    h = NULL;
    t = NULL;
    len = 0 ;
    lists = 0;
    treat = 0;
}
//析构函数
LinkQueue::~LinkQueue()
{
    Node * ptr = NULL;
    while (head != NULL )
    {
        ptr = head;
        head = head->next;
        delete ptr ;
    }
}
//输入函数
void LinkQueue::Input()
{
    ElemType e;
    e.Input();
    if(e.getQue() == 0)
        Ordinary(e);
    if(e.getQue() == 1)
        Emergency(e);
}
//输出函数
void LinkQueue::Output(ElemType e)
{
    e.Output();
}
//普通病人入队
bool LinkQueue::Ordinary(ElemType e)
{
    QNode * ptr = new QNode ;
    ptr->data = e;
    ptr->next = NULL;
    if (tail != NULL )
    {
        tail->next = ptr;
    }
    else 
    {
        head = ptr ;
    }
    tail = ptr ;
    len++;
    lists++;
    return true;
}
//急诊病人入队
bool LinkQueue::Emergency(ElemType e)
{
    PNode * p = new PNode ;
    p->data = e;
    p->next = NULL;

    if (t != NULL )
    {
        t->next = p;
    }
    else 
    {
        h = p ;
    }
    t = p ;
    len++;
    treat++;
    return true;
}
//普通病人出队
bool LinkQueue::pop1()
{
    if(isEmpty1())
        return false;
    QNode *ptr = head ;
    ElemType e;
    e = ptr->data;
	
    Output(e);
    head = head->next;
    delete ptr ;
    ptr = NULL;
    if (head == NULL )
    {
        tail = NULL ;
    }
    return true;
}
//急诊病人出队
bool LinkQueue::pop2()
{
    if(isEmpty2())
        return false;
    PNode *p = h ;
    ElemType e;
    e = p->data;
//	e.Output();
    Output(e);
    h = h->next;
    delete p ;
    p = h;
    if (head == NULL )
    {
        t = NULL ;
    }
    return true;
}
//获取头元素
ElemType LinkQueue::front()
{
    if (this->isEmpty1() == true )
    {
        printf("the Queue is empty!!" );
        return head->data;
    }
    return head->data;
}
//判断队列是否为空
bool LinkQueue::isEmpty1()
{
    return head==NULL && tail == NULL;
}
//判断队列是否为空
bool LinkQueue::isEmpty2()
{
    return h==NULL && t == NULL;
}
//医护人员登录系统
void LinkQueue::enroll()
{
    char user[]="doctor",a[7];
    char enroll[]="123456",b[7]; //用户名密码初始为doctor,123456
    int i;
    int num=0;//控制循环变量

    while(num<3) //密码验证程序
    {
        printf("\t请输入你的工作通行证：\n");
        printf("\t你总共有3次机会\n");
        printf("\t你现在还有%d次机会\n",3-num);
        printf("\t用户名：");
        for(i=0;i<6;i++)
        {
            a[i]=getchar();
        }
        getchar();
        a[6]='\0';
        printf("\t密码：");
        for(i=0;i<6;i++)
        {
            b[i]=getch();
            putchar('*');   //用*来回显密码
        }
        b[6]='\0';
        getchar();
        if((strcmp(user,a)==0)&&(strcmp(enroll,b)==0))      // 验证输入的用户名，密码是否正确
        {
            printf("\t用户认证成功！\n\n");
            success=1;
            break;
        }
        else
        {
            printf("\n\t用户名或密码错误！\n\n");
            system("cls");              //清屏
            success=0;
        }
        num++;
    }
    if(num==3)                      //错误输入三次，将不允许再输入
    {
        printf("\t对不起，你输入的次数已达上限~\n");
        printf("\t用户验证错误，登录失败！");
        printf("\t请按任意键退出!\n\n");
        exit(0);
    }
}
//医生就诊系统
void LinkQueue::Doctor()
{
    static char memory='1';

    if(memory != 'y' && memory != 'Y')  //保存密码的功能
    {
        enroll();
        printf("\t记住密码请输入y或Y,否者输入其他：");
        memory=getchar();
        getchar();
        printf("\n\n");
    }
    if(success == 1)
    {
        while(1)
        {
            if(len == 0)
            {
                system("cls");//清屏
                printf("\t现在暂时没有病人排队就医！\n");
                printf("\t请等待或按1退出就诊系统 +--  ");
                char be[5]="1";

               // scanf("%s",&be);
				cin>>be;
                getchar();
                if(strcmp(be,"1")!=0)
                {
                    continue;
                }
                else
                    break;

            }
            else
            {
                system("cls");
                printf("\t现在排队就诊的有%d个人 \n",len);

                if(treat>0)
                {
                    printf("\t就诊的病人信息如下：\n\n");
                    pop2();
                    treat--;
                }
                else
                {
                    printf("\t就诊的病人信息如下：\n\n");
                    pop1();
                    lists--;
                }
                printf("\t就诊完毕请输入任意键(按1退出医诊系统~) +--  ");
                char ae[5]="1";
                gets(ae);

                if(strcmp(ae,"1")!=0)
                {   
                    len--;
                }
                else
                {
                    len--;
                    break;
                }   

            }
        }
    }
}
int main()
{
    int z = 0;//就诊人数
    int menu;//菜单选择
    LinkQueue qu;
    while(1)
    {
        printf("\n\n           +--------------------------------------------+\n");
        printf("           |           欢迎来到本医院排队就诊           |\n");
        printf("           +--------------------------------------------+\n\n");
        printf("           +--------------------------------------------+\n");
        printf("           |                  1、挂号系统               |\n");
        printf("           |                  2、医生诊治               |\n");
        printf("           |                  0、退出系统               |\n");
        printf("           +--------------------------------------------+\n\n");
        printf("           +-------请选择您要的功能:");
   
		cin>>menu;
        getchar();  
        system("cls");
        switch(menu)
        {
        case 0:
            exit(1);
        case 1:
            qu.Input();
            system("pause");
            break;
        case 2:
            qu.Doctor();
            system("pause");
            break;
        default:
            printf("\t+-------------------输入错误!----------------+\n\n");
            getch();  //密码以不回显方式输入函数（getch();）         
            system("cls");//暂停
            break;
        }
        system("cls");
    }
    system("pause");
    return 0;
}
