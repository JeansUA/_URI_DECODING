# _URI_DECODING
#include "stdafx.h"
#include <stdlib.h>
#include <string.h>
#include <STRING>
#include <stdio.h>
#include <iostream>
using namespace std;
int _tmain(int argc, _TCHAR* argv[])
{
	int count=0;
	char ** arrData;
	cout<<"Enter Count : ";

	//cin>>count;
	count = 3;
	string data1 = "%20";
	string data1_1 = " ";
	string data2 = "%21";
	string data2_1 = "!";
	string data3 = "%24";
	string data3_1 = "$";
	string data4 = "%25";
	string data4_1 = "%";
	string data5 = "%28";
	string data5_1 = "(";
	string data6 = "%29";
	string data6_1 = ")";
	string data7 = "%2a";
	string data7_1 = "*";
	string arData="";
	int pos;
	printf("Enter URI : \n");
	arrData = (char **)malloc(sizeof(char *)*count);
	
	for(int j=0;j<count;j++)
	{
		arrData[i] = (char *)malloc(sizeof(char)*80);

		cin>>arrData[i];

		arData = arrData[j];
		while((pos = arData.find(data1)) != string::npos){
			arData.erase(pos,data1.length());
			arData.insert(pos, data1_1);
		}
		while((pos = arData.find(data2)) != string::npos){
			arData.erase(pos,data2.length());
			arData.insert(pos, data2_1);
		}
		while((pos = arData.find(data3)) != string::npos){
			arData.erase(pos,data3.length());
			arData.insert(pos, data3_1);
		}
		while((pos = arData.find(data4)) != string::npos){
			arData.erase(pos,data4.length());
			arData.insert(pos, data4_1);
		}
		while((pos = arData.find(data5)) != string::npos){
			arData.erase(pos,data5.length());
			arData.insert(pos, data5_1);
		}
		while((pos = arData.find(data6)) != string::npos){
			arData.erase(pos,data6.length());
			arData.insert(pos, data6_1);
		}
		while((pos = arData.find(data7)) != string::npos){
			arData.erase(pos,data7.length());
			arData.insert(pos, data7_1);
		}
		cout<<arData<<endl;
	}
	
	return 0;
}
