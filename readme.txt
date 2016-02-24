					
					***COMMAND LINE TOOL***
		40201757 - Dimitar Hristov - BSc (Hons) Computing Science
		
	This Command Line Tool can find a particular string in a piece of text. In order to work the tool takes a number of arguments.
	The arguments that can be used are the word they are searching for, '-i','-o' and '-c'. More details below.
	The user has two options in order to enter a text:
	
	1) The first option is to use an input file. In this case, the user must the '-i' argument. 
	After the '-i' they must specify the name of the file, they want to use. For example, if we are looking for the word "time" 
	in the input file "book.txt", the whole command will look like: "find time -i book.txt". You can find another example in the 
	makefile as "test3". In this case the result is printed to the standard output, as we have not provided any output file.
	If we want to store the results from the search in a "output.txt" file we must use the '-o' argument. For example,
	in order to store the output from the a search in a "output.txt" file, we have to write "find time -i book.txt -o output.txt".
	You can find another example in the makefile as "test0". Remember that if you type in some of the arguments '-i' or '-o'
	you must enter the name of the file. Otherwise the Command Line Tool will stop and it will give you an error message.
	
	2)The second option to enter a text to search in is the Standard Input. In this case, the user will have to use some CMD commands.
	For example, you can type in command such as "tasklist" or "dir" and they will provide the text to search in. If you want to use this Command Line Tool
	to check if a particular program is currently running on your computer, for example chrome, you can type in "tasklist | find chrome". 
	You can find another example in the makefile as "test9". Here we have not provided any output file, so by default the results are printed on the Standard Output. 
	If you want to get the search result in a text file,you will have to use the '-o' argument. For example, in order to output the result of a search you can type in 
	"tasklist | find chrome -o output.txt". You can find another example in the makefile as "test10". Remember that if you type in the argument '-o'
	you must enter the name of the file. Otherwise the Command Line Tool will stop and it will give you an error message.
	
	The third arument '-c' is used when you want to ignore the case of the letters while searching. For example, if you use '-c' while searching for the word "HELLO"
	and in the text there is the word "hello", it will show you that there is a match. When writing the command line arguments, it does not matter where you write the '-c' argument.
	If you are looking for the word "brother" in a "book.txt" file and you want to ignore the case, you must write "find brother -i book.txt -c". You can find another example in the 
	makefile as "test1", "test2" and "test4".
	
	NOTE: i) As you can see from example "test5" from the makefile, if you do not input a word to search for, the Command Line Tool will stop and an error message will occure. 
	ii) What is more, as you can see from examples "test6","test7" and "test8" ,if your input file does not exist or is invalid or the output file is invalid or does not exist
	the Command Line Tool will stop and an error message will occure.
	iii) As you can see in example "test11", if you type in CMD command and in the same time enter an input file, the Command Line Tool will read from the input file.