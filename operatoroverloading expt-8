#include<iostream>
#include<string>
#include<list>
using namespace std;
class Youtube_channel{
	public:
	string name;
	int no_of_users;
	public:
	Youtube_channel(string nm, int user){
		name=nm;
		no_of_users=user;
	}	
};
class MyCollection{
	public:
		list<Youtube_channel>mylist;
		void operator+=(Youtube_channel& channel){
			mylist.push_back(channel);
		}		
			
};
ostream& operator<<(ostream& COUT, Youtube_channel& channel){
	COUT<<channel.name;
	COUT<<channel.no_of_users;
	return COUT;
}
ostream& operator<<(ostream& COUT,MyCollection& mc){
	for(Youtube_channel ytc: mc.mylist)
	COUT<<ytc;
	return COUT;
}
int main()
{
	Youtube_channel yc1("Sakshi",5000);
	Youtube_channel yc2("Shravani",6000);
	MyCollection mc;
	mc+=yc1;
	mc+=yc2;
	cout<<mc;
	return 0;
}
