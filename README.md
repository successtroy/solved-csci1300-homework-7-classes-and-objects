Download Link: https://assignmentchef.com/product/solved-csci1300-homework-7-classes-and-objects
<br>
<h1>Objectives</h1>

<ul>

 <li>Understand classes and objects</li>

</ul>

<h1>Questions</h1>

<strong>Question 1: Player Class  </strong>

Create ​Player.h​ and ​Player.cpp​ to implement the Player​        ​ class as described below. You will also need to create a ​playerDriver.cpp​ file to test your Player class implementation.




The ​Player​ class has the following attributes:

<table width="624">

 <tbody>

  <tr>

   <td width="312"><strong>Data members (private): </strong></td>

   <td width="312"> </td>

  </tr>

  <tr>

   <td width="312">name​: ​string</td>

   <td width="312">The player’s name</td>

  </tr>

  <tr>

   <td width="312">points​: ​double</td>

   <td width="312">The player’s points</td>

  </tr>

  <tr>

   <td width="312"><strong>Member functions (public): </strong></td>

   <td width="312"> </td>

  </tr>

  <tr>

   <td width="312">Default constructor</td>

   <td width="312">Set ​name​ to an empty string​             ​ and ​points to value 0.</td>

  </tr>

  <tr>

   <td width="312">Parameterized constructor</td>

   <td width="312">Takes a ​string​ and double​               ​ assigning name​ and ​points​, in this order</td>

  </tr>

  <tr>

   <td width="312">getName()</td>

   <td width="312">Returns the player’s ​name​ as a ​string</td>

  </tr>

  <tr>

   <td width="312">getPoints()</td>

   <td width="312">Returns the player’s ​points​ as a ​double</td>

  </tr>

  <tr>

   <td width="312">setName(string)</td>

   <td width="312">Sets the player’s ​name​ (and returns nothing)</td>

  </tr>

  <tr>

   <td width="312">setPoints(double)</td>

   <td width="312">Sets the player’s ​points​ (and returns nothing)</td>

  </tr>

 </tbody>

</table>




For the zip submissions, the files should be named as ​Player.h​, ​Player.cpp​, and playerDriver.cpp​. Your implementation should be organized nicely into separate files. In your ​playerDriver.cpp​, you should have a main ​main​ where you write test cases for each method (constructor, getters, and setters). ​<a href="https://moodle.cs.colorado.edu/course/view.php?id=1275#section-11">Please check the sample submissions on Moodle</a>




<table width="624">

 <tbody>

  <tr>

   <td width="420">Sample main (Be sure to test all methods!)</td>

   <td width="204">Expected outputs</td>

  </tr>

  <tr>

   <td width="420">Player hector(“Hector”, 6.2);  cout &lt;&lt; hector.getName() &lt;&lt; endl; cout &lt;&lt; hector.getPoints() &lt;&lt; endl;</td>

   <td width="204">Hector6.2</td>

  </tr>

 </tbody>

</table>




For the code runner, paste your Player class and its implementation (both ​Player.h​ and

Player.cpp​)







<strong>Question 2: Team Class  </strong>

Create ​Team.h​ and ​Team.cpp​ to implement the Team​          ​ class as described below. You will also need to create a ​teamDriver.cpp​ file to test your ​Team​ class implementation.




The ​Team​ class has the following attributes:

<table width="624">

 <tbody>

  <tr>

   <td width="312"><strong>Data members (private): </strong></td>

   <td width="312"> </td>

  </tr>

  <tr>

   <td width="312">teamName​: ​string</td>

   <td width="312">The team’s name</td>

  </tr>

  <tr>

   <td width="312">players​: an array of ​Player​ objects of size 50</td>

   <td width="312">The players on this team</td>

  </tr>

  <tr>

   <td width="312">numPlayers:int</td>

   <td width="312">The number of players stored in the array</td>

  </tr>

  <tr>

   <td width="312"><strong>Member functions (public):</strong></td>

   <td width="312"> </td>

  </tr>

  <tr>

   <td width="312">Default constructor</td>

   <td width="312">Set ​name​ to an empty string​             ​ and numPlayers to 0</td>

  </tr>

  <tr>

   <td width="312">Parameterized constructor</td>

   <td width="312">Takes a string to initialize ​teamName​  and sets numPlayers to 0.</td>

  </tr>

  <tr>

   <td width="312">setTeamName(string)</td>

   <td width="312">Takes a ​string​ to set teamName​     ​ (and returns nothing)</td>

  </tr>

  <tr>

   <td width="312">readRoster(string)</td>

   <td width="312">Takes the file name (a ​string​), reads a list of player names and their points values, and stores them into the ​players​ array for this team. It returns the number of players in the file as an ​integer​.</td>

  </tr>

  <tr>

   <td width="312">getPlayerName(int)</td>

   <td width="312">Returns the ​name​ (​string​) of the player at position ​i​ within the ​players​array</td>

  </tr>

  <tr>

   <td width="312">getPlayerPoints(int)</td>

   <td width="312">Returns the ​points​ (​double​) of the player at position ​i​ within the ​players​ array</td>

  </tr>

  <tr>

   <td width="312">getNumPlayers()</td>

   <td width="312">Returns the number of players on this team(as an ​integer​)</td>

  </tr>

  <tr>

   <td width="312">getTeamName()</td>

   <td width="312">Returns the name of this team ( ​string​)</td>

  </tr>

 </tbody>

</table>




<em>Method specifications</em>​:

Team​ Class Method: ​<strong>readRoster(string)</strong>​: It takes a file name and reads a list of players and their points separated by a comma. Each player should be stored into the ​players​ array. The function returns the number of players stored in the array. If the file cannot be opened, it should return -1.







Sample file (<u>​</u><a href="https://moodle.cs.colorado.edu/pluginfile.php/214590/mod_folder/content/0/roster1.txt?forcedownload=1"><strong>roster1.txt</strong></a>​):

O’Flaherty,5.5

Ioana Fleming,6.1

Patil,8

Ku,4.9

Sankaralingam,1.7







Team​ Class Method: ​<strong>getPlayerName(int)/</strong>​ ​<strong>getPlayerPoints(int)</strong>​: They take the index of a player object within the ​Player​ array.




For ​<strong>getPlayerName(int)</strong>​<strong>, </strong>it returns the name of the player at the given index. If the index is​    invalid, then it returns “ERROR”.




For ​<strong>getPlayerPoints(int)</strong>​<strong>, </strong>​it returns the point of the player at the given index. If the index is invalid, then it returns -1.




<em>What’s an invalid index?</em>​  An invalid index means that there is no player at that  index. There are two cases in which this can occur: 1) The index is greater than or equal to the number of players in the team.  2) the index is greater than the size of the array.







For the zip submissions, the files should be named as ​Team.h​, ​Team.cpp​, and teamDriver.cpp​. Your implementation should be organized nicely into separate files. In the main​, you should have test cases to test all of your functions.




<table width="624">

 <tbody>

  <tr>

   <td width="420">Sample main (Be sure to test all methods!)</td>

   <td width="204">Expected outputs</td>

  </tr>

  <tr>

   <td width="420">// Using <a href="https://moodle.cs.colorado.edu/pluginfile.php/214590/mod_folder/content/0/roster1.txt?forcedownload=1">roster1.tx</a><u>​        </u><a href="https://moodle.cs.colorado.edu/pluginfile.php/214590/mod_folder/content/0/roster1.txt?forcedownload=1">t</a> from Moodle​         Team team1(“Seg Faultline”); cout &lt;&lt; team1.getTeamName() &lt;&lt; endl; team1.readRoster(“roster1.txt”); int n1 = team1.getNumPlayers(); cout &lt;&lt; n1 &lt;&lt; endl; for (int i = 0; i &lt; n1; i++) {     cout &lt;&lt; team1.getPlayerName(i) &lt;&lt; “ ”;     cout &lt;&lt; team1.getPlayerPoints(i) &lt;&lt; endl; }</td>

   <td width="204">Seg Faultline5O’Flaherty 5.5Ioana Fleming 6.1Patil 8Ku 4.9Sankaralingam 1.7  </td>

  </tr>

 </tbody>

</table>




For the code runner, paste your ​Player​ class and its implementation and ​Team​ class and its implementation (both ​Team.h​ and ​Team.cpp​)

<strong>Question 3: the game() function  </strong>

Write a function, game, that takes two Team objects as parameters and returns the name of the winning team.




<em>Function specifications:  </em>

<ul>

 <li>The function name: <strong>game</strong>​</li>

 <li>The function takes two parameters, both of the type Team​ .​</li>

 <li>The function returns the name of the winning team, as a string​</li>

</ul>

○    To determine the winning team, add up the points associated with each team’s first 4 players. The team with more points is the winner.

○    If one or both of the teams do not have 4 or more players, your function should return “forfeit”

○    If the teams have the same total points, your function should return “draw”

○    The output of “forfeit” takes higher priority than “draw” in the sense that if a team doesn’t have enough players, a game cannot be played, so there could be no draw (for example, if both teams have no players, this would constitute a “forfeit”, not a draw).




Example1, the team Seg Faultline wins because the total points of their first 4 players is 24.5 points, whereas Team Maim only has 21.9 points.




<table width="624">

 <tbody>

  <tr>

   <td width="420">Sample main (Be sure to test all methods!)</td>

   <td width="204">Expected outputs</td>

  </tr>

  <tr>

   <td width="420">// Using <a href="https://moodle.cs.colorado.edu/pluginfile.php/214590/mod_folder/content/0/roster1.txt?forcedownload=1">roster1.tx</a><u>​ </u><a href="https://moodle.cs.colorado.edu/pluginfile.php/214590/mod_folder/content/0/roster1.txt?forcedownload=1">t</a> and ​  <a href="https://moodle.cs.colorado.edu/pluginfile.php/214590/mod_folder/content/0/roster2.txt?forcedownload=1">roster2.tx</a><u>​ </u><a href="https://moodle.cs.colorado.edu/pluginfile.php/214590/mod_folder/content/0/roster2.txt?forcedownload=1">t</a>// from MoodleTeam team1(“Seg Faultline”); team1.readRoster(“roster1.txt”); Team team2(“Team Maim”); team2.readRoster(“roster2.txt”); string winner = game(team1, team2); cout &lt;&lt; “The winner is: ” &lt;&lt; winner &lt;&lt; endl;</td>

   <td width="204">The winner is: Seg Faultline </td>

  </tr>

 </tbody>

</table>




The file name should be named gameDriver.cpp​ . In your main, make sure that you call the​      function and output the return value.




For Coderunner, paste your Team​       and ​     Player​              classes and their implementations, and your​ game function (submit what you did for Problems 2 and 3, and add your ​   game​    function).​