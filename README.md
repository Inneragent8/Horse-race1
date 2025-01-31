advance(int horseNum, int* horses)
printLane(int horseNum, int* horses)
isWinner(int horseNum, int* horses)
displayRace(const vector<int>& positions)
raceFinished(const vector<int>& positions)

function 1:
advance(int horseNum, int* horses)

horseNum (int): The number of the horse (between 0 and 4).
horses (int*): An array representing the positions of all horses. Each horse's position is stored at index i.
steps:
Check if the horse is allowed to advance.
Increment the position of the horse by 1, if the horse is allowed to move.
Return nothing.
output: Modifies the horses array to reflect the updated position of the specified horse.

function 2:
printLane(int horseNum, int* horses)

horseNum (int): The number of the horse whose lane is being printed.
horses (int*): An array representing the positions of all horses.
Steps:
Loop through each position in the horses array to print out the lane.
For the specified horseNum, print the position on the track as a number (the horse itself).
For all other horses, print a dot (.) to represent empty spaces in their lanes.
After printing one lane for the specified horse, print a new line.
output: A single line representing the track position of the horse specified by horseNum with other horses in their corresponding lanes.

function 3: 
isWinner(int horseNum, int* horses)

horseNum (int): The number of the horse to check.
horses (int*): An array representing the positions of all horses.
Steps:
Check if the specified horse’s position is greater than or equal to TRACK_LENGTH - 1.
If it is, return true, indicating this horse is a winner.
if not, return false.
output: A boolean value (true or false) indicating whether the horse has reached or surpassed the finish line.

function 4: 
displayRace(const vector<int>& positions)

positions (const vector<int>&): A vector of integers representing the current position of each horse.
Steps:
Loop through all horses (from 0 to NUM_HORSES - 1).
For each horse, print the track.
Loop through the positions vector.
If the current index matches the horse's position, print the horse's number.
Otherwise, print a dot (.) for empty space.
Print a new line after each horse's track.
Print a blank line after displaying all the horses.
output: A visual display of the race, with each horse's position shown on the track.

function 5:
raceFinished(const vector<int>& positions)

positions (const vector<int>&): A vector of integers representing the current position of each horse.
Steps:
Loop through each horse's position in the positions vector.
If any horse's position is greater than or equal to TRACK_LENGTH - 1, return true, indicating that the race is finished.
If no horse has finished, return false.

output: A boolean value (true or false) indicating whether the race is over.

algeritem:
Initialize the random number generator.
Create a vector positions to store the positions of each horse.
Display a welcome message and prompt the user to start the race.
While the race is not finished:
For each horse, randomly decide if it should move forward.
Update the position of the horses.
Display the current state of the race.
Prompt the user to press Enter to continue.
After the race ends, display a message indicating the race is over.
