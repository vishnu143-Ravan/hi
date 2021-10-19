lab2:
LAB SESSION 02:
Date of the Session: / / Time of the Session: to
Pre-Lab:
1) Given a text txt[0..n-1] and a pattern pat[0..m-1], write a function search (char pat [], char
 txt[]) that prints all occurrences of pat[] in txt[] using naïve string algorithm?(assume that n > m)
Input
txt[] = "THIS IS A TEST TEXT"
pat[] = "TEST"
Output
Pattern found at index 10
Input
txt[] = "AABAACAADAABAABA"
pat[] = "AABA"
Output
Pattern found at index 0
Pattern found at index 9
2) Discuss the Rabin Karp algorithm for string matching and explain time complexity of the
algorithm?
3) Stefan is a guy who is suffering with OCD. He always like to align things in an order. He got a lot
of strings for his birthday party as gifts. He like to sort the strings in a unique way. He wants his
strings to be sorted based on the count of characters that are present in the string.
Input
 aaabbc
 cbbaaa
Output
aabbcc
aabbcc
If in case when there are two characters is same, then the lexicographically smaller one will be printed
first
Input:
aabbccdd
aabcc
 Output:
 aabbccdd
 baacc
In-Lab:
1) Naive method and KMP are two string comparison methods. Write a program for Naïve
method and KMP to check whether a pattern is present in a string or not. Using clock
function find execution time for both and compare the time complexities of both the
programs (for larger inputs) and discuss which one is more efficient and why?
 Sample program with function which calculate execution time:
#include<stdio.h>
#include<time.h>
void fun()
{
//some statements here
}
int main()
{
//calculate time taken by fun()
clock_t t;
t=clock();
fun();
t=clock()-t;
double time_taken=((double)t)/CLOCK_PER_SEC; //in seconds
printf(“fun() took %f seconds to execute \n”,time_taken);
return 0;
}
2) Andrea is working in a photo studio where his boss has given him a task to arrange the
photos of family members. He is French and he do not know English somehow, he managed
to send the list of names to you (his friend). Help Andrea to sort the photos.
(Note: implement the odd even merge algorithm)
Input
5
Neil Katherine Harry Stefan Dennis
Output
Dennis Harry Katherine Neil Stefan
Post-Lab:
1) Given a pattern of length- 5 window, find the valid match in the given text by step-by-step
process using Robin-Karp algorithm
Pattern: 2 1 9 3 6
Modulus: 21
Index: 0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21
Text: 9 2 7 2 1 8 3 0 5 7 1 2 1 2 1 9 3 6 2 3 9 7
2) James is sharing his information with his friend secretly in a chat. But he thinks that
message should not understandable to anyone only for him and his friend. So he sent the
message in the following format.
Input
 a1b2c3d4e
Output
abbdcfdhe
Explanation:
The digits are replaced as follows:
- s[1] -> shift('a',1) = 'b'
- s[3] -> shift('b',2) = 'd'
- s[5] -> shift('c',3) = 'f'
- s[7] -> shift('d',4)

lab3
==============
Pre-Lab:
1) Write a Divide and Conquer algorithm to find the minimum distance between the pair of the points
given in an array. Find the time complexity of the algorithm.
P[] = {{2, 3}, {12, 30}, {40, 50}, {5, 1}, {12, 10}, {3, 4}}
2) Write a divide and conquer algorithm for finding the maximum and minimum in the sequence of
numbers. Find the time complexity.
3) Trace out the output of the following using Merge sort.10, 49, 32, 67, 45, 4, 7, 2, 1, 51, 78, 34, 89,
87, 36, 29, 3, 9, 11.
In-Lab:
1) Harry’s Aunt and family treat him badly and make him work all the time. Dudley, his cousin got
homework from school and he as usual handed it over to Harry but Harry has a lot of work and his
own homework to do.
The homework is to solve the problems which are numbered in numerical he tries to solve random
question after solving random questions he did not put those questions in order Dudley will return
in a time of n*logn Harry has to arrange them as soon as possible. Help Harry to solve this
problem so that he can go on and do his own homework.
Example
Input
9
15,5,24,8,1,3,16,10,20
Output
1, 3, 5, 8, 10, 15, 16, 20, 24
2) A group of 9 friends are playing a game, rules of the game are as follows: Each member will be
assigned with a number and the sequence goes like e.g.: 7,6,10,5,9,2,1,15,7.
Now they will be sorted in ascending order in such a way that tallest one will be sorted first. Now
your task is to find the order of indices based on initial position of the given sequence and print the
order of indices at the end of the iteration.
19CS3113S ANALYSIS & DESIGN OF ALGORITHMS
Post-Lab:
1) Suppose a merge sort algorithm, for input size 64, takes 30 secs in the worst case. What is the
maximum input size that can be calculated in 6 minutes (approximately)?
2) Chris and Scarlett were playing a block sorting game where Scarlett challenged Chris that he has to
sort the blocks which arranged in random order. And Scarlett puts a restriction that he should not use
reference of first, median and last blocks to sort, and after sorting one block with reference to other
block, for next iteration he must choose another block as the reference not the same block (random
pivot).
Now, Chris wants help from you to sort the blocks. He wanted to sort them in a least time. Help him
with the least time complexity sorting algorithm.
Input format
First line of input contains the number of test cases.
Next t lines of input contain
The number of blocks provided by Scarlett.
lab4:
===========) Trace the output of the following matrix multiplication using Strassen’s Multiplication Method
A, B and C are the Matrices of Size NxN
a, b, c and d are the sub-Matrices of A of size N/2xN/2
e, f, g and h are the sub-Matrices of B of size N/2xN/2
2) China had recently banned cryptocurrency. Due to this cryptocurrency cost has fallen drastically. Mr.
Lee has lost a lot so he could not afford a stock advisor. He came to you (his friend) for help. He has
the prices of stock on i’th day. Help him to find the maximum profit he can achieve. You may
complete as many transactions as you like.
Input
7
[1,2,3,4,5,6,7]
Output
6
Explanation:
Buy the stock on 1st day at cost 1Rupee and sell 
In-Lab:
1) You are given 2 matrices of any size N*N. Write a program to find the product of the two matrixes
(use Strassen’s Matrix Multiplication).
2) Mr. Lee is working in a construction where they had to fencing around trees in a field. The owner
has asked a rough estimate to do fencing in that field such all the trees lie inside that region.
Consider yourself as a cost estimator who works under Mr. Lee. You are given location of all the
trees, and you need to find the points that include this fencing. You need to output the trees that
are included in the fencing.
Input:
points = [[1,1], [2,2], [2,0], [2,4], [3,3], [4,2]]
Output:
[[1,1], [2,0], [3,3], [2,4], [4,2]]
3) In a school there was conducted a contest among two groups. As part of the contest each group
must re-arrange the cards that had given to the members in ascending order. Consider yourself as a
part of the team and find the best viable way to win that round.
Input
3
3
[[2,5,6], [4,8,7], [9,3,1]]
Output
[1,2,3,4,5,6,7,8,
1) Mr. Hari Kumar owns a fruit market. In the market there are many sellers who are selling many kinds
of fruits. More than one fruits seller can sell same kind of fruit. Mr. Hari Kumar wants to arrange their
information in the sorted order based on their names of the sellers and id of the fruits. You must
arrange the same type of fruits in the same order as original order.
0-mangoes 1-apples
[Hint: Use counting sort algorithm]
Input
4
[[0, c], [1, b], [0, a], [1, d]]
Output
[[0, a], [0, c], [1, b], [1, d]]
2) Given a set of points in the plane, apply convex hull algorithm to the given points and explain it step

==================
===========================lab5:==========================================
1) Explain why 0-1 Knapsack problems cannot be solved using greedy method unlike fractional
knapsack.
2) Categorize the Following as single source or multiple source shortest path algorithms.
Floyd-Warshall algorithm
Dijkstra’s algorithm –
Bellman-Ford algorithm –
3) List down various shortest path greedy algorithms.
19CS3113S ANALYSIS & DESIGN OF ALGORITHMS
In-Lab:
1) Given an array of size n that has the following specifications:
a. Each element in the array contains either a police officer or a thief.
b. Each police officer can catch only one thief.
c. A police officer cannot catch a thief who is more than K units away from the police officer.
 We need to find the maximum number of thieves that can be caught.
Input
arr [] = {'P', 'T', 'T', 'P', 'T'},
k = 1.
Output
2
Here maximum 2 thieves can be caught; first police officer catches first thief and second police
officer can catch either second or third thief.
2) Given n non-negative integers a1, a2, ..., an, where each represents a point at coordinate (i, ai). n
vertical lines are drawn such that the two endpoints of the line i is at (i, ai) and (i, 0). Find two lines,
which, together with the x-axis forms a container, such that the container contains the most water.
The program should return an integer which corresponds to the maximum area of water that can be
contained (maximum area instead of maximum volume sounds weird but this is the 2D plane we are
working with for simplicity).
Notice that you may not slant the container.
 Input: array = [1, 5, 4, 3]
 Output: 6
 Explanation :
 5 and 3 are distance 2 apart. So the size of the base = 2. Height of container = min(5, 3) = 3.
 So total area = 3 * 2 = 6
 Input: array = [3, 1, 2, 4, 5]
 Output: 12
 Explanation :
 5 and 3 are distance 4 apart. So the size of the base = 4. Height of container = min(5, 3) = 3.
 So total area = 4 * 3 = 12
Input
height = [1,8,6,2,5,4,8,3,7]
Output
49
19CS3113S ANALYSIS & DESIGN OF ALGORITHMS
Post-Lab:
1) Given an array of jobs where every job has a deadline and associated profit if the job is finished
before the deadline. It is also given that every job takes a single unit of time, so the minimum
possible deadline for any job is 1. How to maximize total profit if only one job can be scheduled at
a time.
Input
4
Job ID Deadline Profit
a 4 20
b 1 10
c 1 40
d 1 30
Output
60
profit sequence of jobs is c, a
2) There are N Mice and N holes are placed in a straight line. Each hole can accommodate only 1
mouse. A mouse can stay at his position, move one step right from x to x + 1, or move one step
left from x to x − 1. Any of these moves consumes 1 minute. Assign mice to holes so that the time
when the last mouse gets inside a hole is minimized.
 Example: positions of mice are: 4 -4 2
 Positions of holes are: 4 0 5
 Input:
 A: list of positions of mice
 B: list of positions of holes
 Output:
 single integer value
 ====================================lab6==================================================
 Pre-Lab:
1. Our TASC has the information that a scientist has gone crazy and was planning a gas
leakage in Delhi. We do not know the exact location where he was planning to do this
attack. When Srikanth Tiwari tried to catch him, The Scientist tried to kill himself and
has gone into coma in this process. Now no one knows the location of the attack except
he has kept all the information in a file in his private server, but it is encoded using
Huffman coding. So, help NIA decode the information. Given the root of the graph and
the encoded information write a function to decode it. The function will have input
parameters of root node and encoded string.
Input
Encoded String-1001011
Output
ABACA
In-Lab:
1) You are a Human resource manager working in a Startup. You are tasked with to utilize the
best of the working professionals to get the maximum profit for different jobs of a Project.
An array of jobs is given where every job has a deadline and associated profit if the job is
finished
before the deadline. It is also given that every job takes single unit of time, so the minimum
possible
deadline for any job is 1.How to maximize total profit if only one job can be scheduled at a
time.
Write a code for the following problem.
Input
7
a b c d e f g
3 4 4 2 3 1 2
35 30 25 20 15 12 5
Output
110
d c a b
2) Surya is a student at KL University, He is currently standing in the C-Block. He has 8 friends
who are situated at different Blocks (Places) inside the university and he wishes to talk to
each of them in person. The distances are represented on the undirected graph which is
provided below. He wishes to take the shortest distance for each place from his location.
Help him in meeting every one of his friends by developing a program that can determine the 
shortest distance between the C-Block and every other place on the graph. Remember that
the path is not required.
Hint: Use Dijkstra’s algorithm to calculate the distances between the C-Block and every
other place
Output for the same is provided along with the question.
Output:
Vertex Distance from Source
C Block 0
FED Block 4
S Block 12
Main Canteen 19
Entrance 21
Xerox 11
R&D Block 9
Mech Block 8
Library 14
Post-Lab:
1. Mr. Tripathiis a network cable operator. He now shifted to a new city where he needs to
work on designing the cable lines to each street/colony. Given the graph and each node
represents a street, help him to design an optimal cable line using prim's algorithm. Write a
program to solve this.
2. Mr.Tripathi done with designing the cable lines but now there comes 
============================lab7=========================================================================
Pre-Lab:
1) A student named Satish is eagerly waiting to attend tomorrow’s class. As he searched the concepts of
tomorrow’s lecture in the course handout and started solving the problems, in the middle he was
stroked in the concept of strings because he was poor in this concept so help him so solve the problem,
given two strings str1 and str2 and below operations that can performed on str1. Find minimum
number of edits (operations) required to convert ‘str1’ into ‘str2’.
1. Insert
2.Remove
3.Replace
Input
str1 = "cat", str2 = "cut"
Output
1
We can convert str1 into str2 by replacing 'a' with 'u'.
Input
str1 = "sunday", str2 = "saturday"
Output
3
2) Given N numbers n1,n2,…nN and Q queries q1,q2,…qQ. Your task is to print Q (Q< j <numbers)
f1,f2,…fQ, corresponding to query qj1 max(n1=fj ,n2 ,...nq) using dynamic programming.
Input
5 3
5 4 8 6 9
2 3 5
Output
5 8 9
In-Lab:
1) Bhanu is a student at KL University who likes playing with strings, after reading a question from their
lab workbook for the ADA Course she found what is meant by a subsequence.
(A subsequence is a sequence that can be derived from another sequence by deleting some or no
elements without changing the order of the remaining elements)
So, she created 2 strings out of which one she considered as a master string and the other one as a slave
string. She challenged her friend Teju to find out whether the slave string is a subsequence of the master
string or not, As Teju is undergoing her CRT classes she decided to code the logic for this question.
Help her in building the logic and write a code using Dynamic programming concept.
2) Geeta is working in a company, and she has n different projects to work on, where every project is
scheduled to be done from startTime[i] to endTime[i], obtaining a profit of profit[i]. You are given the
startTime, endTime and profit arrays, return the maximum profit you can take such that there are no
two projects that she is working on in that given subset with overlapping time range. If she chooses a
project that ends at time a then she will be able to start another project that starts at time b.
Input
startTime = [1,2,3,4,6], endTime = [3,5,10,6,9], profit = [20,20,100,70,60]
Output
19CS3113S ANALYSIS & DESIGN OF ALGORITHMS
150
Explanation: The subset chosen is the first, fourth and fifth project.
Profit obtained 150 = 20 + 70 + 60.
3) Teacher: good morning students!!!
Students: good morning mam
Teacher: Today topic is binary tree. Does anyone know what is binary tree?
Students: no mam
Teacher: In computer science, a binary tree is a tree data structure in which each node has
at most two children, which are referred to as the left child and the right child. Satish you
completed this topic yesterday can you explain this topic?
Satish: Sure, mam but I got doubt this concept, do anyone help me in solving this the question was
Given a binary tree, find whether if a given Binary Tree is Balanced?
Post-Lab:
1) SIRI studies at KL University and a person who is interested in Dynamic Programming, she created a
question for you to solve. she decided to give a question related to palindrome, you need to use
dynamic programming to solve this problem brute force is not allowed since she hates waiting too
long to find the answer. The question follows like this find the longest palindromic subsequence.
(Unlike substrings, subsequences are not required to occupy consecutive positions within the original
string.)
Input
ABBDCACB
Output
The length of the longest palindromic subsequence is 5
The longest palindromic subsequence is BCACB
2) Bhanu and Teju are playing dice game where there are N dice with M faces and the dice are numbered
from 1 to M. A person wins the game if the sum of the faces of dice adds up to a value X. you are
playing on Bhanu’s team, and It is Teju’s turn now.
You are supposed to find number of ways your opponent can win the game where N, M and X are
provided as input. Use Dynamic programming to solve the problem.
Using DP (Dynamic programming) to find the number of ways to get sum X.
Input
M = 2
N = 2
X = 3
Outp
=======================lab9=================================================
What is Back Tracking methodology and when can we use Back tracking, explain with an example?
2) Mr. Anumula went to the Ice-Cream Parlor. He will be with certain amount of money to buy icecreams. When he goes to the counter for ordering the Ice-cream, there will be displayed with the
items and its cost, respectively. He will be checking which items he can buy according to the
money. Print "YES" if he can buy the Ice-Creams without leaving one rupee also otherwise print
"NO".
Input
costs= [100, 70, 50, 180, 120, 200, 150]
Total Money=300
Output
 YES
In-Lab:
1) Mani is poor at playing chess, he was asked to arrange “N” Queens on the chess board in such a
way that no two queens are allowed to kill each other. Since he is poor at chess you were asked to
arrange them on behalf of him. (You must use Backtracking Approach)
2) Given an undirected graph and N colors, the problem is to find if it is possible to color the graph
with at most N colors, which means assigning colors to the vertices of the graph such that no two
adjacent vertices of the graph are colored with the same color.
Print "Possible" if it is possible to color the graph as mentioned above, else print "Not Possible".
Input
1
3 2
0 2
1 2
2
Output
 Possible
Post-Lab:
1) Kiran is a very obedient boy and helping others is a habit of him. He will do any work with dedication
his teacher assigns him a work to generate all permutations of given word. Since he is busy helping
others, you are asked to help him to complete his work on behalf of him. (Use Backtracking Concept)
19CS3113S ANALYSIS & DESIGN OF ALGORITHMS
2) Mr. Sai joined for as an assistant at a school where he was given a job to arrange schedules for the
subject n1, n2, n3, n4, n5, n6, n7, n8. Help him schedule the timetable from the given information.
Let this be the schedule:
Here for everyone hour there are many subjects competing. Use backtracking and create a schedule
where each subject is assigned to a specific hour in a day. In the schedule ‘1’ represents that the 
=========================================lab8=========================================================
Pre-Lab:
1) Your father brought you a ticket to world tour. You have a choice to go to three places, your father
knows the places you wanted to travel so he made a graph with the measuring distances from home.
Now you start from your place (1: Source) to other places as shown in the graph below apply TSP to
find shortest path to visit all places and return to home. (Ex: 2: London, 3: Paris, 4: Singapore)
2) You are given a map(graph) with the distances between the places. Here you will consider the 1st
node as the starting point and ending point, Since the route is cyclic you can take any node as starting
point and ending point. Find the minimum cost route and remember the Hamiltonian cycle.
3) Your friend works in a comparable way to a Travelling salesperson ― he always travels to new cities
to sell his delicious dishes.
Today, your friend is planning to visit N cities (numbered 1 through N). There is a direct way to travel
between each pair of cities. Each city has a specific temperature; let us denote the temperature in the ith city by Ci. Your friend has a fixed temperature tolerance D with the following meaning: for each
pair of cities an and b, he may travel from city a directly to city b only if |Ca−Cb|≤D, otherwise he
would catch a heavy flu because of the sudden change in temperature.
Your friend starts from city 1. Is he able to visit all N cities in such a way that each city is visited
exactly once?
Notes:
1. Your friend is not able to travel through a city without visiting it.
2. City 1 is visited at the beginning.
It is not necessary to be able to travel directly to city 1 from the last city Your friend’s visits.
Input
2
5 3
19CS3113S ANALYSIS & DESIGN OF ALGORITHMS
3 2 1 4 5
5 4
10 1 3 2 9
Output
Yes
No
In-Lab:
1) Emma has a graph which represents a flow network where every edge has a capacity. Also given
two vertices source s and sink t in the graph, fin the maximum possible flow from s to t with
following constraints:
a. Flow on an edge does not exceed the given capacity of the edge.
b. Incoming flow is equal to outgoing flow for every vertex except s and t.
Find the Maximum flow using the graph and by implementing the code.
2) For the above given graph Emma wants an s-t to cut that requires the source s and the sink t to be
in different subsets, and it consists of edges going from the source’s side to the sink’s side. So, she
wants you to find the minimum capacity s-t cut of the given network. Expected output is all the
edges of minimum cut.
Post-Lab:
1) Hogwarts has yet again declared The Triwizard tournament. Harry must pass this round to get to
the next one. Each participant will be given a graph with vertices as shown below. Each vertex is a
dungeon, and a golden egg is placed in the root dungeon i.e., the root vertex. Help harry find the
dungeon with the golden egg using traversing or searching tree or graph data structure. (P.S: To
pass this round Harry must write a code).
2) KL University is starting next week. There are S subjects in total, and you need to choose K of
them to attend each day, you required number of credits to pass the semester. There are N+1
buildings. Your hostel is in building number 0. Subject j is taught in building Bj. After each
subject, you have a break, during which you go back to your hostel. There are M bidirectional
paths of length 1 which connects building b1 to building b2. Find the minimum total distance you
need to travel each day if you choose your subjects correctly.
Input
2 3 2 2
0 1
1 2
2 0
1 2
Output


