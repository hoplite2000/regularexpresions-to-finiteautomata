# Compiler Design Assignment on - “Conversion of regular expression to NFA, DFA and minimal DFA”

## OPERATING ENVIRONMENT

### Hardware Requirements

	1. Operating System: Ubuntu 16.04 LTS or higher, Windows 7 or higher.
	2. Processor: 1.8 Ghz or faster processor
	3. RAM: 0.6GB or more

### Software Requirements

	1. g++ Compiler
	
	g++ command is a GNU c++ compiler invocation command, which is used for preprocessing, compilation, assembly and linking of source code to generate an executable file. The different “options” of g++ command allow us to stop this process at the intermediate stage. 

### List of related files 
	1. C++ file - regex.cpp <br>
	2. Executable file - ./a.out <br>
	
### Procedure to compile and run

	g++ regex.cpp
	./a.out	

	Terminate the program with CTRL+Z or any other key.

	-std=c++11 or any other version can be given as an option to while executing the code.


## SAMPLE TEST CASES <br>
	Enter Regular Expression: ab*
	Postfix Expression: ab*.



	---------------------------------------
	Input Regex: ab*

	1. NFA
	2. Intermediate DFA
	3. Minimized DFA
	4. Simulation
	Press any other key to exit...

	1


	Phase 1: regex to nfa conversion
	------------------------------------------------------------------------
	State	|	a	|	b	|	eps	|accepting state|
	------------------------------------------------------------------------
	0	|	1 	|		|		|	No	|
	1	|		|		|	4 	|	No	|
	2	|		|	3 	|		|	No	|
	3	|		|		|	2 5 	|	No	|
	4	|		|		|	2 5 	|	No	|
	5	|		|		|		|	Yes	|
	------------------------------------------------------------------------

	---------------------------------------
	Input Regex: ab*

	1. NFA
	2. Intermediate DFA
	3. Minimized DFA
	4. Simulation
	Press any other key to exit...

	2

	NFA TO DFA CONVERSION
	---------------------------------------------------------
	STATE	|	a	|	b	|	FINAL	|
	---------------------------------------------------------
	0	|	1	|	3	|	0	|
	1	|	3	|	2	|	1	|
	2	|	3	|	2	|	1	|
	3	|	3	|	3	|	0	|
	---------------------------------------------------------

	---------------------------------------
	Input Regex: ab*

	1. NFA
	2. Intermediate DFA
	3. Minimized DFA
	4. Simulation
	Press any other key to exit...

	3
	---------------------------------------------------------
	State	|	A	|	B	|	Final	|
	---------------------------------------------------------
	0	|	0	|	0	|	No	|
	1	|	0	|	1	|	Yes	|
	2	|	1	|	0	|	No	|
	---------------------------------------------------------

	---------------------------------------
	Input Regex: ab*

	1. NFA
	2. Intermediate DFA
	3. Minimized DFA
	4. Simulation
	Press any other key to exit...

	4

	---------------------------------------
	Input Regex: ab*

	1. NFA
	2. Intermediate DFA
	3. Minimized DFA
	4. Simulation
	Press any other key to exit...

	Enter string : aa
	-----------------------------------------
	Input	|	Current	|	Next	|
	-----------------------------------------
	a	|	2	|	1	|
	a	|	1	|	0	|
	-----------------------------------------

	Verdict: Rejected

	---------------------------------------
	Input Regex: ab*

	1. NFA
	2. Intermediate DFA
	3. Minimized DFA
	4. Simulation
	Press any other key to exit...

	4

	---------------------------------------
	Input Regex: ab*

	1. NFA
	2. Intermediate DFA
	3. Minimized DFA
	4. Simulation
	Press any other key to exit...

	Enter string : abbb
	-----------------------------------------
	Input	|	Current	|	Next	|
	-----------------------------------------
	a	|	2	|	1	|
	b	|	1	|	1	|
	b	|	1	|	1	|
	b	|	1	|	1	|
	-----------------------------------------

	Verdict: Accepted

	---------------------------------------
	Input Regex: ab*

	1. NFA
	2. Intermediate DFA
	3. Minimized DFA
	4. Simulation
	Press any other key to exit...	
	
	CTRL+Z 
