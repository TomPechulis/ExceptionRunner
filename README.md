# ExceptionRunner
1) It is different because the logger makes sure to log where and what is requested within the program itself. "Finer"loging level is always outputted to the log,not console, unlike INFO.

2) This comesfrom the Timer Exception that is thrown because of the filOverTest() that passes -1 to Timer.timeMe.

3)Asserts the execution for the given executable that throws an exception and returns the exception.

4) 
	1. The serialVersionUID is a unique identifier for Serializable classes that is used during the desrialization of an object to make sure that a loaded class is compatible with the serialized object.

	2. We need to override contsructors because unlike the @Before tag, constructors force you to call the parent class constructors and exceptions in the constructor dont cause the @After methods to be called.
	3. The parent class handles the other methods, so we dont need to for those methods. This lets the parent class functionality to work in the subclass.

5) The static block is ran once every time the class is loaded into memory. It is useful for setting up the logging since it would then apply to every instance of that class.


6)The .md file format means that the file is a Markown file. Markdown has its own sytanx and when it comes to the README.md in BitBucket, it can also contain a restricted set of HTML tags.

7) The test was failing due to the NullPointerException being thrown because of the finally statement, since it throwing the timer exception didnt completely exit out of the program. This caused the -1 in timeToWait to still be used later in the program. 
I fixed this issue by just removing the finally statement since it causes the null value to still be used in the method, when it shouldnt be. 

8) The actual issue here is that a nullpointerException is not handled when it should be.



11) A TimerException extends Exception which makes it a checked exception. 
A NullPointerException extends RuntimeException which makes it an unchecked exception.
