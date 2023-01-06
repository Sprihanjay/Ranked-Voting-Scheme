
# Ranked Voting Scheme (CSC 1301 Projects)
Write a Python program to implement the Ranked Voting scheme. In this modified voting scheme, each ballot lists 1st preference, 2nd preference, etc. The voting ballots are again present in a text file with each line corresponding to a single ballot. The candidates are listed in preference order and are separated by commas. Here is a sample input file:
<pre>
mirage:02-vote raj$ more vote2.dat 
Red,Green
Blue
Green,Red,Blue
Blue,Green,Red
Green
The method to determine the winner proceeds by eliminating candidate(s) with lowest number of 1st choice votes (if there are ties, eliminate all). 
This process is repeated until a single candidate remains. That candidate is declared the winner. 
If by eliminating candidates in any one round no candidate remains then all the candidates remaining in that round are declared the winner.
Mac-mini:02-vote raj$ python3 Vote2.py vote2.dat 
Ballots:  [['Red', 'Green'], ['Blue'], ['Green', 'Red', 'Blue'], ['Blue', 'Green', 'Red'], ['Green']]
Winner:  Green
</pre>
