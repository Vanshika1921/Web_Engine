# Web_Engine
1.It is a web engine project made using C++. Wherein you can search a an issue and it redirects you to SOLUTION page

2.This is a program that takes user input in the form of a search query, searches for relevant problems in a file, and provides solutions to the most relevant problem based on the search results.

3.The code defines two classes: 'Generic_Problem' and 'Solutions'. Solutions inherits from Problems.

4.The 'Problems' class has a member function 'differentProblems()' that prompts the user to enter a search query and returns the user's input as a string.

5.The 'Solutions' class extends the 'Problems' class. It has several member functions, including 'Life_solution()', 'subSearch()', and 'printQuestions()'. The 'Life_solution()' function reads a file ('Generic_Problem.txt') line by line, filters the lines based on a search query, and stores the matching lines in a
vector. The 'subSearch()' function processes the filtered lines, counts the occurrences of each line, and displays the most frequent line along with its frequency. It also reads URLs from another file ('Generic_Solutions.txt') and opens the URL corresponding to the most frequent line using the 'openURL()' function. The 'printQuestions()' function is not implemented in the code.

6.he 'openURL()' function uses the Windows API function 'ShellExecuteA()' to open a URL in the default browser.

7.In the 'main()' function, the user's search query is obtained using the 'differentProblems()' function. The query is split into individual words and stored in an array.

8.The 'Life_solution()' and 'subSearch()' functions are called to search for relevant problems and display the most frequent problem's solution, respectively.
