# android-app-performance
Coding practice to increase performance of Android App


##Performance Tips
1. Avoiding Unnecessary Object Creation
2. Creating static methods
3. Creating final static variables
4. Using Enhanced for Loop
5. Minimizing access to private methods from inner class
6. Using int where possible.

##1. Avoiding Unnecessary Object Creation
Method using unnecessary variable
```java
private String getString(String name){
	String helloString="Hello " + name;
	return helloString;
}

```
After Changes above code
```java
private String getString(String name){
	return "Hello " + name;
}

##2. Creating static methods
Normal method 
```java
private String getString(String name){
	return "Hello " + name;
}

```
Not accessing any fields of the class so made this static
After Changes above code
```java
private static String getString(String name){
	return "Hello " + name;
}
```
Reference 
Link ["The Code City": Optimize Android App Performance - Efficiency Tips](https://www.youtube.com/watch?v=wCeSYRwNP50).
