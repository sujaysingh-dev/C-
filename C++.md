``` DATE - 09/25/2024 ```

T. INHERITANCE :-
	Inheritance is the one of the most important powerful feature  in oops,  the main advantage of using code reusability. which achieved by creating new classes from existing classes.
		Inheritance is a feature or a prosses in which new classes created from the existing 
	classes the new classes is called derived class (child class) and existing class is known as base class (parent class) the derive class now is set to be inherited from the base class derive class inherit base class it means the derive class inherit all the properties of the base class without changing the properties of base class and may add new features to its own. this the features in the derived class will not affect the base class.
	
```
Syntax of derived class :- 
class derived_class_name:access specifier base_class_name
{
	-----------
	-----------
	-----------
}
NOTE :- THERE ARE THREE TYPE OF ACCESS SPECIFIER (PUBLIC, PROTECTED, PRIVATE)
```

```
1.	Example of derived class :-
	class A
	{
		protected:
			int x;
		
	};
	class B: public A
	{
		private:
			int y;
	};
	int main()
	{
		A objA;
		B objB;
		cout<<"The size of objA = "<<sizeof(objA)<<endl;
		cout<<"The size of objB = "<<sizeof(objB)<<endl;
	}

2.	Example of derived class :-
	class A
	{
		protected:
			int x, y;
		public:
			void getdata()
			{
				cout<<"Enter the 1st value = "<<endl;
				cin>>x;
				cout<<"Enter the 2nd value = "<<endl;
				cin>>y;
			}
			
	};
	class B : public A
	{
		private:
			int z, sum;
		public:
			void setdata()
			{
				cout<<"Enter the 3rd value = "<<endl;
				cin>>z;
			}
			void add()
			{
				sum = x + y + z;
				cout<<"Sum of these number = "<<sum<<endl;
			}
	};
	int main()
	{
		B objB;
		objB.getdata();
		objB.setdata();
		ojbB.add();
	}
```

``` DATE - 10/25/2024 ```

