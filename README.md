# Proportional-Representation-Calculator
This is a personal project, and the calculator uses the Sainte-Laguë method to convert the number of votes for each political party into seats in a legislative election. Sainte-Laguë method is a proportional representation method.

## Sainte-Laguë method
The Sainte-Laguë method is used in countries such as Germany, New Zealand, and Sweden. There are many variations of the method's formulas, but the default formula used for the method is "v / (2s + 1)" where "v" is the total number of votes the party earned, and "s" is the number of seats already allocated to that party. This is the formula used in this calculator's algorithm. The party with the highest quotient in the round gets one seat for that round.

## Tibreaker Logic
The calculator features a tiebreaker algorithm. Whenever there are more than one party with the same maximum quotient, the number of votes received is reviewed, and the tied party with more votes is the winner for that round. If the number of votes is tied between the parties, then the victorious party is chosen randomly.

## How to use
Download prCalc.html in the Github repository and open it in VS Code. Then, under "View" at the top menu, click on "Extensions". Then look for a Live Server and install it. Then, right click on prCalc.html on the left-hand menu and click on "Open with Live Server" or "Open with Five Server" depending on what extension you installed. This will bring you to the page in a browser.

The first page you encounter asks you for the number of parties that are participating in the election. Your answer must be an integer greater than 0. Your answer will result in the number of rows for the form.

After you submit that, you will encounter a page asking for:
 - Total number of seats up for election (must be an integer greater than 0), 
 - Electoral threshold: not filling this out will result in the default threshold of 0%. Parties must reach the electoral threshold in order to be awarded seats. Electoral threshold must be either an integer or decimal that is at least 0%.
 - Name of party along with number of votes the party received. You cannot have the same name for more than one party. The number of votes must be an integer at least 0.

Below that, there are four buttons:
  - Go Back: this button brings you back to the page where you are asked for the number of parties.
  - Delete Last Row: deletes the last row in the "party and votes" form.
  - Add Row: adds a row to the bottom of the "party and votes" form.
  - Calculate: calculates the number of seats for each party and displays the results in a table. Summary results are also displayed.

After you press the calculate button, the results will appear at the bottom. You will see the summary results which showcases:
  -  The total number of votes cast in the election.
  -  The total number of seats up for election.
  -  The electoral threshold.
  -  A statement declaring that all parties passed the threshold set. If not, then the parties that failed to reach the threshold are listed here.
  -  Number of parties that participated in the election and the number of parties that were able to win seats.

Below the results summary is the table showing the results. The table has four columns:
 - The name of the party
 - The number of seats the party won
 - The percentage of seats the party won (rounded to two decimal places)
 - The percentage of votes the party won (rounded to two decimal places)

If there is a party that won a majority (> 50%), then the party appears in bold font in the table.

Reminder: remove any commas when inputting numbers. For example, 1,000 should be 1000.
