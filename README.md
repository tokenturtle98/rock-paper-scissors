#Andrew Joel, Mathew 
import random;


w= False #to keep the while loop repeating

#no need for blank space helps me determine where the different modules are

while w == False:
	u = input("Enter your choice (rock/paper/scissors): ");
	u = u.lower(); #changes the choice to lowercase so there are no errors 
	if u == "exit":
		exit();
	cInt = random.randint(0,2); #computer chooses between rock, paper, or scissors
	if (cInt == 0):
		c = "rock";
	elif (cInt == 1):
		c = "paper";
	elif (cInt == 2):
		c = "scissors";
	else:
		c = "Huh? Error...";
	print(c)

#no need for blank space helps me determine where the different modules are

 #covers all the possible scenarios of the game  
	if (u == c): 
		print("Draw!");
	elif (u == "rock"):
		if (c == "paper"):
			print("Computer wins!")
		else:
			print("You win!");
	elif (u == "paper"):
		if (c == "rock"):
			print("You win!");
		else:
			print("Computer wins!")
	elif (u == "scissors"):
		if (c == "rock"):
			print("Computer wins!");
		else:
			print("You win!");



