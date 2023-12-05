# Lab-6b
#include<iostream>
#include<cmath>
#include<ctime>
#include<cstdlib>

using namespace std;

int rollD20()
{
	return rand() % 20 + 1;
}
//This is a very insightful observation re: your code. 
int rollD4()
{
	return rand() % 4 + ;
}

int main()
{
	srand(time(0));

	int d20Result, d4Result;
	int rollCount = 0;

	do
	{
		d20Result = rollD20();
		d4Result = rollD4();

		cout << "Roll #" << ++rollCount << ": d20 = " << d20Result << ", d4 = " << d4Result << endl;
	}

	while (!(d20Result == 1 && d4Result == 1));

	cout << "Snake eyes achieved afrer" << rollCount << "rolls!" << endl;

	return 0;
}








	
