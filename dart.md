# dart


## First code:
<p>
void main() { //standerd function

//code 
 
 print("hello eslam");
 
}

</p>

## null safty


void main(){

  //null safty
  
  // it means i cant declare variable without assign value to it

  String name;

// print(name);//error

  // i can make null varaible with two way

  String? age;

late String info;

  print(age);//null

//if i use method with null varaible will return error if i need to force it i used

//print(age!.length);

}

## Variables:

void main() {
  
  String name ="eslam";
  
  int age = 10;
  
  age=20; //reassign value to variable
  
  print(name);
  
  print(age);

  // there are keywords i cant give it name to variable like Async , await
   
}


## Data type:

void  main() {
  
  // data type
  
  String name ='eslam '; //can i use "" or ''
  
  String lastname="essam salah";

  print (name+lastname); //to concat
  
  print ("$name $lastname"); //another way to merge to variables
   
   int age=20;
  
  double x=20.3;
  
  bool gender=true;
   
}


 
## Arthmetic operators

void  main() {
  
  // arthmetic operators
  
  // add +
  
  //subtract -
  
  //devide / or ~/
  
  //multible *
  
  //mod %

  int a=10;
  
  int b=5;
  
  int c=a~/b; //the result will be int
  
  double e=a/b; //the result will be double
  
  print(c);
  
  print(e);
   
}


## comparison operator

void  main() {
 
 //comparison operator
 
 // == equal
 
 // != not equal
 
 // > bigger than
 
 // < less than

// <= 

// >=

int a=10;

int b=5;

print(a==b);//false

}


## test operators and assign operators

void  main() {

//test operators and assign operators

//test

int x =5;

print(x is int);

print (x is! int); //is not => false


//assign

int a=10;

a ??= 20; //if (a) didnt have any value then assign 20 for it

print(a);

a +=20; // a=a+20;

a -=20; // a=a-20;

a *=20; // a=a*20; and so on

}

## logical operators


void  main() {

//logical operators

// && and

// || or

// ! not


int a=10;

int b=5;

print( a>4 && b>4  );

print( a>4 || b>7  );

print( !(a>4 || b>7 ) );

}

## comments

void  main() {

// comments

// one line comment

/* 

multi

line 

comment

*/

}

## if statment

void  main() {

// if statement

/* 

 if(condtion){

   code

}else if(condtion){
   
   code
 
 }else{

 }

*/

int a=10;

int b=5;

if(a>b){

print("a is bigger than b");

}else{
 
 print("a is not bigger than b");

}

}

## switch statment

void  main() {

// switch statment 

/* 

switch(case){

case 1 :{ code} break;

case 2 :{ code} break;

case 3 :{ code} break;

case 4 :{ code} break;

default :{code}

}

*/

int price=5000;

// can i use curly brackts {} after case like that => case 1 :{ code} break; 

//or without like that  => case 1 : code break;
  
 switch(price){

  case 1000:print("i have 1000 dollar"); break;

  case 2000:{ print("i have 2000 dollar"); } break; // look above
  
  default: print("i have $price dollar")  ;break;

}

}

## for loop

void main(){

// for loop 

// for(var =value ; condtion; step ){code}

 for(int year=1900; year<=2022; year++){ //will print years from 1900 to 2022

  print(year);
 
 }

}

## while loop

void main(){

// while loop 

// while(condtion){code; step}

int year=2000;

while(year>=1900){ //print year from 2000 to 1900

 print(year);

 year--;
  
  }

}

## do while loop

void main(){
 
  int year=2000;

  do{ //in do while loop the code will execute atleast one
   
   print(year);
 
   year--;

 }while(year>=1900); //print year from 2000 to 1900
 
}

## break

void main(){
 
 //break => its mean exit from the loop 
 
  int year=2000;

 while(year>=1900) //print year from 2000 to 1950
  {
   print(year);
  
	if(year==1950){
  
	 break;
    }
   
	 year--;
 
 }
 
}

## continue

void main(){

//contiune => its mean escape one round from the loop 

for(int year=2000; year>=1900; year--) //print year from 2000 to 1900 without 1950

{

   if(year==1950)continue;

    print(year);

 } 
 
}

## numbers

void main(){
 
 //numbers

 int a=10;
 
 print(a.isFinite); // is finite number? true
 
 print(a.isInfinite);// is infinite number? false

 int b=-10;
 
 print(b.isNegative);//is negative number? true
 
 print(b.sign);//it return -1 is negative and 1 is postive and 0 is number is 0

 //even ,odd
 
 print(a.isEven);//true

 //abs
 
 print(b.abs());//absloute value

 //ceil,floor,round
 
 double x=2.3;
 
 print(x.ceil());//will be 3 =>upper number 
 
 print(x.floor());//will be 2 =>lower number 
 
 print(x.round());//will be 2 =>closer number

 //compareTo
 
 print(a.compareTo(10));//if number is equal the number it return 0 
 
 print(a.compareTo(15));//if number is smaller than the number it return -1 
 
 print(a.compareTo(4));//if number is greater the number it return 1


//toint , todouble

int s=10;

print(s.toDouble());//10.0

double d=20.3;

print(d.toInt());//20

//num.pares() to change from String to int

String Q ="10";

print(Q is int);//false

print(num.parse(Q) is int);// true

}

## string

void main(){

//string

String a='eslam ';

int b=10;

print(a + " " + "essam" );//concate string with another

print(a + " " + "$b");//concate string with variable number

print(a + " "+ "${b+150}");//concate string with variable number and make an operation to it 

//isempty

print(a.isEmpty);

//length

print(a.length);

//to uppercase

print(a.toUpperCase());

//to lowercase

print(a.toLowerCase());

//trim

print(a.trim());//move the space

//replaceall

String c="How are you";

print(c.replaceAll("you", "we"));

}

## list 1

void main(){
 
 //list 1 


List names=["eslam","essam",180];

print(names);

print(names[0]);//eslam


List names2=["eslam",[1,2,3,4],"essam",180];

print(names2);

print(names2[1][3]);//4

}

## list 2


void main(){

//list 2

List names=["eslam","essam",1,2,3,4,5];

names[0]="aaa"; //to change the value of index

names[1]="bbb";

names.add("eslam");//to add member to list

print(names);

//to print all members in list

for(int i=0; i<names.length; i++){

  print(names[i]);

}
 
 print("*"*20);

//another method

names.forEach((name) { print(name); });

}


##list 3

void main(){

//list 3

List names=["eslam",'essam', 1 , 2.5 , 3 ];

print(names.first);//eslam  

print(names.last);//3

print(names.isEmpty);//false

print(names.isNotEmpty);//true

print(names.reversed);

print(names.reversed is List);// false

print(names.reversed.toList());

}

## list 4

void main(){

//list 4

List names=["aaa",'bbb',"ccc" , "eee"];

names.add(["eslam" , 'essam']);//add it as a list ,i can use add to add only one item

print(names);

names.addAll([1,2,3,4]);//add it as members ,add more than one item

print(names);

names.insert(0, "mm");//insert one item at specifc index

print(names);

names.insertAll(0, [100,200]); //insert more than one item at specific index

print(names);

} 

## list 5

void main(){

//list 5

List names=["aaa",'bbb',"ccc" , "eee"];

//replaceRange(start, end, replacements)

names.replaceRange(0, 3, [1,2,3]); // will replace 0,1,2 index

print(names);

print("*"*20);

//remove ,removeAt, removeRange

names.remove('eee');//remove by value

print(names);

names.removeAt(0);//remove by index

print(names);

names.removeRange(0, 2);

print(names);

} 

## map

void main(){

//map {key:value}

Map info={"name":"eslam", "age":20 , "country":"egypt"};

print(info);

print(info['name']);//i can access by key

print(info.keys);//to print keys

print(info.values);//ro prtnt values

print(info.isEmpty); //false

print(info.isNotEmpty);//true


//print using foreach

info.forEach((key, value) {

 print("$key $value");

});

//reomve(key)

info.remove("country");

print(info);

//addAll

info.addAll({"price":3000});

print(info);

}

## dynamic variable

void main(){

//dynamic variable

//we know some data type like=> String , int ,bool, double, list , map

//dynamic variable i can assign any data tupe to it

var a=20;

var b="eslam";

var c=[1,2,3,4];//list

var e={"name":"eslam"};//map

print(a);

print(b);

print(c);

print(e);


}

## const and final

void main(){

//const and final

String name="eslam";

name="aa";// notice that i can override it

print(name);

//const

const String info="eg"; //now i cant override it

print(info);

//final

final String country="egypt"; //like const with some different in memory space

print(country);

}

## set

void main(){

  //set 

  Set name={"eslam","essam","ahmed","ahmed"};

//the adventage of set that it must be uniqe

//notice that "ahmed" is written twice but when i print it will appear one time

print(name);

name.add("momen");

name.addAll({1,2,3,4});

print(name);

}

## converting between some data types

void main(){

  //converting between data types

 //set to list or opposite

Set name={"eslam","essam","ahmed"};

print(name.toList());

  List num=[1,2,3,4,5];

print(num.toSet());

  //map to set or list

  Map info={"name":"eslam","age":20};

  print(info.values.toList());

print(info.values.toSet());

}

## function

void main(){

//1-namefunction(parameter){code}

//2-namefunction();

message(){

print("How are you ");

}

message();

sumnum(int a,int b){

int c=a+b;

print(c);

}

sumnum(16, 10);

sumnum(200, 135);

}

## function 2

void main(){

//function return types 1-void 2-return

void message(){

print("How are you "); // void =>print

}

message();

int sumnum(int a,int b){

int c=a+b;

return c ;

}

  int result=sumnum(16, 10);

print(result);

  //notice if i dont assign any return type to function it will be dynamic

}

## import


import 'functions.dart'; //if the file in the same folder 

import '../functions.dart'; //if the file in folder outside main folder

import 'files/functions.dart'; //if the file in the folder his name is (files) inside main folder

void main(){

// i imported it from functions.dart 

sumnumbers(200, 300);

}

## import as


import 'dart:math' as math;

void main(){

//solve example for math equation in 2 degree


int a=2;

int b=4;

int c=1;

double s1;

double s2;

int delta= b * b - 4 * a * c;

 if (delta>0){

   s1= (-b + math.sqrt(delta))/(2*a);

	 s2= (-b - math.sqrt(delta))/(2*a);
 
   print("x1= $s1");
   
	 print("x2= $s2");
 
 }else if(delta==0){
  
	  s1=s2= -b /2*a;
 
 }else{
 
    print("there is no soultions");
 
 }
 
}



## runes


void main(){

//runes integer unicode

String name="eslam";//e=101, s=115 and so on

print(name.codeUnits);

print(name.runes); // the same

 //where i can use it ? if i need to split string to chars //just example i can use (for) as well

 name.runes.forEach((element) {

print(String.fromCharCode(element));

});

 String emoji="\u{1F601}"; //unicode for emoji

print(emoji);
}

 
## assert

void main(){

//assert(condtion ,message)

int a;

assert(a!=null,"a is null ?"); //it use for check about condtion like variable shouldn't be null  

print(a);

}


## max , min

import 'dart:math';

void main(){

//max(), min()

int a=20;

int b=30;

  print(max(a, b));//30

print(min(a, b));//20

}

## advanced data type list ,map, set

void main(){

//data type list ,map,set


List<String> names=["eslam","essam"]; //list conatin string only
  
  Map<String,String> info={ //map contain only string in key and value

"name":"eslam",

"age" :"22"

};

  List<Map<String,String>> infos=[{ //list contain only map that contain only string in key and value

"name":"eslam",

"age" :"22"

  }];

  Set<int> s={1,2,3,4};
 
 }

## some important methods



import 'dart:math';

void main(){
 
 //sublist, shuffle, asMap, whereType ,Firstwhere

  //sublist
 
 List names=["AaA",123,"bbb",15,"ccc",20,"ddd"];

  List sublist=names.sublist(2);//make sublist from list sublist(start,end)
 
 print(sublist);

  //shuffle
 
 names.shuffle();// repalce index rendomly
 
 print(names);

  //asMap

  Map maplist=names.asMap();//convert list to map
 
 print(maplist);

  //whereType
 
 var numbers=names.whereType<int>();//return all numbers in the list and i can specifie the data type 
 
 var string=names.whereType<String>();
 
 print(numbers);
 
 print(string);

  //whereFirst

  var x=names.firstWhere((element) => element >100);//return the first element where condtion is true //(=>) means return
 
 print(x);

}


## some important methods 2

import 'dart:math';

void main(){

//any ,every ,take

List names=["eslam","essaam",1,2,3,4];

var x=names.any((element) => element.length >3);//return true or false if the condtion executed for any element

print(x);

  var x2=names.every((element) => element.length >5);//return true or false if the condtion executed for every element

print(x2);

  var x3=names.take(3);//return the elements depends on number i gave it =>("eslam","essaam",1)

print(x3);

}


## some important methods 3

void main(){

//where , indexWhere

List names=["aaa","bbb","ccc"];

  var x1=names.where((element) => element.length >2);// it return all element that have executed the condtion

print(x1);

  var x2 =names.indexWhere((element) => element.length >2);//it return the index of the first element that executed the condtion

print(x2);

}

## some important methods 4



void main(){

//startWith, endWith ,contain , indexOf

String names="eslam";

    var x1=names.startsWith("e");//return true or false if the string starts with "e"

print(x1);

    var x2=names.endsWith("s");//return true or false if the string ends with "s"

print(x2);

    var x3=names.contains("es");//return true or false if the string contains "es"

print(x3);

    var x4=names.indexOf("a");//return the index of "a"

print(x4); 

}


## iterable , iterator



void main(){

/* 

Iterable

[1] objects contains data that can be iterated upon

[2] Examples [list , set]

    Iterator

[1] Object used to iterate over Iterable using MoveNext() method return 1 element at A time

[2] You can generate iterable from iterator method

[3] Loops already called iterator

[4] Gives stop iteration if there is no Move Next element 

*/

  List names=['eslam','essam','ahmed','mohamed'];//iterable

  Iterable names2=['eslam','essam','ahmed','mohamed'];//iterable => list

  Iterable names3={'eslam','essam','ahmed','mohamed'};//iterable => set
 
  for(String name in names){ //loop ==iterator

    print(name);
  
	}

  Iterator itr =names.iterator; // [2]

  while(itr.moveNext()){ //[1]
  
		print(itr.current);
  
	}
 
 }


## try , catch


void main(){
 
 // try and catch 
 
 //used for handling errors

  int a=10;
 
 int b=0;
 
 int c=2;
 
 try{
 
 int res= a ~/c;
 
 print(res); //5

  int errorres=a ~/b ; //will occured error devision by zero
 
 print(errorres);
 
  }catch(e){
 
 			print("Error: $e");
 
 }

}


## short hand if statement


void main(){
  
	// short hand if statement 

  int a=10;

  (a > 5) ? print("a is greater than 10") : print("a is less than 10");

  String name="eslam";

  (name=="ahmed") ? print("name is eslam") : print("name is not eslam");

}


## oop



class Moblie{

//var

String name="";

double screen=0.0;

//constractor

Moblie(String name,double screen){

	this.name=name;

	this.screen=screen;
 
 }
 

//method
  
	void printInfo(){
  
	print("Your phone is : ${this.name} \nYour screen large is : ${this.screen} ");
 
 }

}

void main(){
 
 // oop

  Moblie mobile1=new Moblie("samsung",5.6);// make an object
 
 mobile1.name="Iphone"; //access object variables and method
 
 mobile1.screen=6.4;
 
 print(mobile1.name); 
 
 mobile1.printInfo();
 
 //another example

 Moblie moblie2=new Moblie("redmi 6",6.9); //passing a properties by constractor
 
 print(moblie2.name);
 
 print(moblie2.screen);
 
 moblie2.printInfo();  

}


## reset varaibles

class User{

//var

String name="";

int phone=0;

// 3-

User(this.name, this.phone);

}

void main(){
 
  // 1- user1.name="eslam";

	// 2- cascade operator => User user1=new User()..name;
  
			//  User user1=new User()..name="eslam";
  
			//print(user1.name);

  // 3-cosntractor
  
	  //User(this.name, this.phone);

 User user1=new User("eslam", 123456);
 
 print(user1.name);

 // 4- setter and getter

}


## setter and getter 

class User{
 
 //var
 
 String name="";
 
 int phone=0;

 // constractor
 
 User(this.name, this.phone);

 //setter and getter
 
 void set changeName(String name){ //setter
 
 	this.name=name;
  
	}

  String get newName{ //getter
  
	return this.name;
  
	} 


}

void main(){

// setter and getter

User user1=new User("eslam",123);

user1.changeName="ahmed";

 print(user1.newName);

}

## static

class User{

//var

//i cant access the name via instance (object)

static  String name="eslam";


}

void main(){
// static

	User user1=new User();

//print(user1.name);//error

// but i can access it via class

print(User.name);

}


## cascade operator

class Mobile{
 
 void testone(){

		print("Method one");
 
 }

 void testtwo(){
 
 print("Method two");
 
 }

}

void main(){

// cascade operator
 
//  Mobile mob=new Mobile();

//  mob.testone();

//  mob.testtwo();

new Mobile()..testone()..testtwo();

}

## inheratence

class Mobile{

String screen="";

String camera="";

String cpu="";

String memory="";

 void printinfo(){

		print("mobile father class");
 
 }

}

class samssung extends Mobile{

	String brand ="samssung";

}

void main(){
  samssung s21=new samssung();

  s21.camera="20 mpx";
  	
	s21.cpu="snapdragon 665";

  print(s21.brand);
  
	print(s21.camera);
  
	print(s21.cpu);

  s21.printinfo();


}

## override


class Mobile{
 
 String screen=""; 

 void printinfo(){
 
 		print("mobile father class");
 
 }

}


class samssung extends Mobile{

//override var 

String screen='3.1';

//override method

  @override

void printinfo() {

		print("from child class");
  
	}

}

void main(){
	
	samssung s21=new samssung();

 print(s21.screen);
 
 s21.printinfo();

}

## multi level inheratence

class one{

String onevar="one";

}

class two extends one{ //inherate from one 

String twovar="two";

}

class three extends two{ //inherate from two and two inherate from one so that three will inherate from two and one

String threevar="three";

}



void main(){

three th =new three();

 print(th.onevar);

print(th.twovar);

print(th.threevar);

}

## super class

class one{

final String name;

one(this.name);

 void printInfo(){

		print("parent class");

 }

}

class two extends one{ //inherate from one 
 two(name) : super(name); // super refer to parent class //and here i make constarctor to send name to parent constractor 

@override
  
	printInfo() {
  
		// TODO: implement printInfo
  
		return super.printInfo(); //will return super print info
  
	}

}



void main(){

	two x=new two("eslam");

	x.printInfo();

}

# implements


	abstract class Person{
 
 	String name="eslam";
 
 	String age="";
 
 xyz(){
  
  }

}

class Students implements Person{ // when i use implement i have to use all properties from parent class without there value
	
	String name="";
 
 	String age="";
 
 	xyz(){
  
		print("hello");
 }

}

void main(){

}


## enum



enum status{ // used to store some static words
	
	offline,
  
	online

}

void main(){
 	
	//enum 
 
 status statusCurrent= status.offline;

 if(statusCurrent==status.online){
  
	print("user is online");
 
 } else{
 
 	print("user is offline");
 
 }

}

## regular expression


void main(){
 
 // regular expression
 
 // used to check for validation of input like email
 
 String emailPattern=r"^[a-zA-Z0-9.a-zA-Z0-9.!#$%&'*+-/=?^_`{|}~]+@[a-zA-Z0-9]+\.[a-zA-Z]+"; //google it to get pattern

 RegExp regExp=new RegExp(emailPattern);

 String NotValidemail="eslam.com";

 print(regExp.hasMatch(NotValidemail)); //return false
 
 String validemail="eslam@hotmail.com";
 
 print(regExp.hasMatch(validemail)); //return true


 //validation for phone number like above with change of pattern

}

## private

class User{
 
 	var name="eslam";

  //private variable i cant access it from another file
  
	var _email="eslam@gmail.com";

//private method => i cant access it from another file

_printInfo(){

print("$name  $_email");

}

//privat constarctor

User._(this.name);

User.name():
	name="basel";//defualt initilization to name when using privat constarctor 

}

void main(){

User user=new User.name(); //using private constractor with default init
 
 print(user.name);//basel

}

## mixin , with


mixin one{ //like abstract
	
	var name="eslam";

}

class Two{

var password="156454154";

} 

class Three with one ,Two{ // if i need inherate from more than one class i use  with

}

void main(){

  Three three=new Three();

  print(three.name);

	print(three.password);

}
