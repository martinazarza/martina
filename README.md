# martina.
september 14

Today I will talk about this project that I did for my programming class. I wrote a program where I read a text file containing a student's name and their grades . the goal of this lab is to learn how to use and link files with our program. We also learned to use the if and else statement methodology.

To begin with, let me explain what it is and in what situations we could use the if and else statement, also use char on this occasion. “In c++ character type variables are declared with the char keyword. Only one character can be stored in a character variable. Now let me explain what if and else is all about.
“We can use if and else statement to run one block of code under certain conditions and another block of code under different conditions. “For example in this project we use if and else to see the grades of a student depending on the percentage of it.
If the percentage is greater than or equal to 90 the program will run the letter A;
if the percentage is greater than or equal to 80 the letter will be B;
if the percentage is greater than or equal to 70 the letter will be C;


--The first step was get the variables: 
  ifstream inFile;
   ofstream outFile;
    string fName,lName;
    float g1,g2,g3,g4,g5;
    float avg;
    char lGrade;
--The step 2 was open files :
    inFile.open("grades.txt");
    outFile.open("avg_score.txt");
-- The step 3 was  read from file :
    inFile >> fName >> lName >> g1 >> g2 >> g3 >> g4 >> g5;
    The step 4 was calculate avg and implement logic to generate letter grade
    avg = (g1 + g2 + g3 + g4 + g5)/5;
  --  and then we started to do the calculation with the if and else statement
    if (avg >= 90){
    	lGrade = 'A';
	}else if (avg >= 80){
		lGrade = 'B';
	}else if (avg >= 70){
		lGrade = 'C';
	}else if (avg >= 60){
		lGrade = 'D';
	}else{
		lGrade = 'F';
	}
   -- Then we got the results in step 5 and we printed them 
    cout << fName << " " << lName << " " << avg << " " << lGrade;
    outFile << fName << " " << lName << " " << avg << " " << lGrade; 
    last step was close files
    inFile.close();
    outFile.close();
This is a very common example but also very effective when it comes to wanting to learn and understand the logic of the if and else statement.
