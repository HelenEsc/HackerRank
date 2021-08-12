1. C#: Team Interface
Implement inheritance as described below.

Create a class Team that has the following:

A member variable teamName [string]
A member variable noOfPlayers [integer]
A constructor function:
It takes 2 parameters and assigns them to _teamName _and _noOfPlayers _respectively.
A member function AddPlayer(count):
It takes an integer count as a parameter and increases noOfPlayers by count.
A member function RemovePlayer(count):
It takes an integer count as a parameter and tries to decrease _noOfPlayers _by count.
If decreasing makes noOfPlayers negative, then this function simply returns false.
Else, decrease noOfPlayers by count and return true.
Create a class Subteam that inherits from the above class Team. It has the following:

A constructor function:
It takes 2 parameters, _teamName _and noOfPlayers, and calls the base class constructor with these parameters.
A member function ChangeTeamName(name):
It takes a string name as a parameter and changes teamName to name. 
Note: Declare all the members as public so that they are accessible by the stubbed code.

Your implementation of the function will be tested by a stubbed code on several input files. Each input file contains parameters for the function calls. The functions will be called with those parameters, and the result of their executions will be printed to the standard output by the stubbed code.

Input Format For Custom Testing
The first line contains a string, teamName, and integer, noOfPlayers, denoting the team name and the initial number of players in the team, respectively.

The second line contains an integer, count, which is the parameter for the AddPlayer function.

The third line contains an integer, count, which is the parameter for the RemovePlayer function.

The fourth line contains a string, name, which is the parameter for ChangeTeamName function.

Sample Case 0
Sample Input For Custom Testing
OldTeam 2
3
4
NewTeam
Sample Output
Team OldTeam created
Current number of players in team OldTeam is 2
New number of players in team OldTeam is 5
Current number of players in team OldTeam is 5
New number of players in team OldTeam is 1
Team name of team OldTeam changed to NewTeam
Explanation
First, a team is created with teamName as 'OldTeam' and noOfPlayers as 2. Then, the AddPlayer function is called with parameter 3, so the new noOfPlayers becomes 5. Then, the RemovePlayer function is called with parameter 4, so the new noOfPlayers becomes 1. Finally, the ChangeTeamName function is called with parameter 'NewTeam', which changes teamName to 'NewTeam'.

Sample Case 1
Sample Input For Custom Testing
Champions 2
1
2
IPL
Sample Output
Team Champions created
Current number of players in team Champions is 2
New number of players in team Champions is 3
Current number of players in team Champions is 3
New number of players in team Champions is 1
Team name of team Champions changed to IPL
Explanation
First, a team is created with teamName as 'Champions' and noOfPlayers as 2. Then, the AddPlayer function is called with parameter 1, so the new noOfPlayers becomes 3. Then, the RemovePlayer function is called with parameter 2, so the new noOfPlayers becomes 1. Finally, the ChangeTeamName function is called with parameter 'IPL', which changes teamName to 'IPL'.