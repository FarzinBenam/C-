//a class declaration and fucntion definition in the class. 
#include <iostream>
#include <string>

using namespace std;
//////////////////////////////////////////////
// Declaring a class, bettre beggins with Caps
class Test {
	// only accessable inside the class
	private:
		int age = 25;
	
	// accessable from outside of the class
	public:
		
		string name;
		void num (int number);
		void old (){
			cout << ", " << age << "years old";
		}
		void introduce(){
			cout << "I'm " << name;
			old();
		}
		void newline (){
			cout << endl;
		}
};
// declare a class funct outside of class
//(The :: (scope resolution) operator)
void Test::num (int number){
		cout << number << "-";
	}

string name[] = {"Farzin", "Somaye", "Azaam"};
//////////////////////////////////////////////
int main (){
	int i;
	string name[] = {"Ali", "Hasan", "Husen"};
	
	// these objects are stored in the stack (always static)
	Test obj_1,  obj_2, obj_3;
	// when defined by pointer stored in hip (always dynamic)
	Test *ptr = new Test();
	
	cout << "Normal Object declaration:" << endl;
	for(i = 0; i < 3; i++){
		// normal object access by .
		obj_1.num(i);
		obj_1.name = ::name[i];
		obj_1.introduce();
		obj_1.newline();
	}	
	
	cout << "Pointer Object declaration:" << endl;
	for(i = 0; i < 3; i++){
		// pointer accessed by -> 
		ptr->num(i);
		ptr->name = name[i];
		ptr->introduce();
		ptr->newline();
	}
	
	// others usage of the :: (scope resolution) operator
	// access to a global variable -> change Farzin to METALWORLD
	cout << "use of scope resolution (::) on global var:" << endl;
	::name[1] = "METALWORLD";
	cout << ::name[1] << endl;
	cout << name[1] << endl;
	
	return 0;
}
 
