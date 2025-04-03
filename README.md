#include <iostream>
#include <cmath>
double f(double x1,double y1,double x2,double y2){
    x1-=x2;
    y1-=y2;
    return sqrt(x1*x1+y1*y1);
}
 
double d(double a, double b, double c){
    return a+b+c;
}
 
using namespace std;
 
int main() {
    double x1,y1,x2,y2,x3,y3;
    cin>>x1>>y1>>x2>>y2>>x3>>y3;
    cout << "Периметр: " << d(f(x1,y1,x2,y2),f(x3,y3,x2,y2),f(x1,y1,x3,y3));
}

#include <iostream>

using namespace std;
int main() 
{
    int a, b, c;
    cout << "Введите число:" << endl;
    cin >> a;
    b = a / 10;
    c = a % 10;
    cout << ((b + c) % 2 == 0 ? "Нет" : "Да") << endl;
    return 0;
}

#include <iostream> 
#include <math.h> 
using namespace std; 
int main() 
{ 
double p; 
double S; 
cin >> p; 
S=p / 3.0 * sqrt(3.0) /4.0; 
cout << S << endl; 
return 0; 
}

#include <iostream>
using namespace std;
 
int main()
{
    double x, y, f;
    
    do
    {
    cout <<"x="; cin >> x;
    if (x==-34);
    }
    while (x==-34);
    
    do
    {
    cout <<"y="; cin >> y;
    if (y==-1);
    }
    while (y==-1);
    
    f=(x+y)/(y+1)-(x*y-12)/(34+x);    
 
    cout <<"f="<<f<<endl; 
    return 0;
}

#include <iostream>
using namespace std;
int main()
{
    int x;
    cin >> x;
    switch (x)
    {
        case 1: case 2: case 3: case 4:
        case 5: cout <<"рабочий день"; break;
        case 6: case 7: cout << "выходной"; break;
        default: cout << "вы ошиблись";
}
return 0;
}

#include <iostream>
using namespace std;

void f (const int *b, int &c)
{
    (*b) += 10; // 1
    c+= 10;
}

int main ()
{
    int y = 20, z=30;
    f(&y, 2); // 2
    cout << "main:\t" << y << "\t" << z << endl;
    return 0;
}

#include <iostream>
using namespace std;

void f (int a, int *b, int &c) // определение функции f
{
    a += 10;
    (*b)+= 10;
    c += 10;
    cout << "f:\t" << "\t" <<*b << "\t" << c << endl;
}

int main()
{
    int x = 10, y = 20, z = 30;
    cout << "main:\t" << x << "\t" << y << "\t" << z << endl;
    f(x, &y, z); // вызов функции f
    cout << "main:\t" << x << "\t" << z << endl;
    return 0;
}

#include <iostream>
using namespace std;

float max(float x, float y); // обьявление функции

int main() // главная функция
{
    float a = 5.5, b = 3.2, c = 14.1, d;
    d = max(max(a,b),с); // 1
    cout << "max = " << d << endl;
    return 0;
}

float max(float x, float y) // определение функции
{
    return (x > y) ? x : y;
}

#include <iostream>
using namespace std;
int main()
{
    int x;
    cout << "введите x";
    cin >> x;
    (x % 2 == 0)? cout << "четное\n": cout << "нечетное\n";
    return 0;
}

#include <iostream>
#include <iomanip>
#include <math.h>
using namespace std;
int main()
{
    int x;
    double y;
    cin >> x;
    y = (pow(x,2) + sin(x+1))/25; // 1
    cout << "y= " << setprecision(5) << y << endl;
    return 0;
}

#include <iostream>
using namespace std;
int main()
{
    int a = 1500000000;
    a = (a * 10) /10; // 1 - неверный результат
    cout << "a = " << a << endl;
    int b = 1500000000;
    b = (static_cast<double>(b) * 10) / 10; // 2 - верный результат
    cout << "b = " << b << endl;
    return 0;
}

#include <iostream>
using namespace std;
int main()
{
    int a = 100, b;
    float c = 4.5, d;
    d = a/c; // 1 - без потери точности
    cout << "d= " << d << endl;
    b = a/c; // 2 - с потерей точности
    cout << "b= " << b << endl;
    return 0;
}

#include <iostream>
using namespace std;
int main()
{
    int x, y, max;
    cin >> x >> y;
    cout << (x > y ? x : y) << endl; // 1
    max = x > y ? x : y; //2
    cout << max << endl;
    return 0;
}

#include <iostream>
using namespace std;
int main()
{
   cout << "x \t y \t && \t ||" << endl;
   cout << "0 \t 0 \t" << (0&&0) << "\t" << (0||0) << endl;
   cout << "0 \t 1 \t" << (0&&1) << "\t" << (0||1) << endl;
   cout << "1 \t 0 \t" << (1&&0) << "\t" << (1||0) << endl;
   cout << "1 \t 1 \t" << (1&&1) << "\t" << (1||1) << endl;
   return 0;
}
