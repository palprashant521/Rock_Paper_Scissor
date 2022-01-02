# Rock_Paper_Scissor



import random

print("***Welcome to the Game of Rock-Paper-Scissor***")

choice = 0

user_name = input('Please enter your name:  ')

print('\n')

print(" Please choose: \n 1. Rock \n 2. Paper \n 3. Scissor")

while True:
    
    print('\n')
    choice = int(input('Enter your choice: '))
    print('\n')
    
    while choice<0 and choice>3:
        
        choice = int(input('Enter a valid input: '))
        
    if choice == 1:
        
        choice_name = 'Rock'
        
    elif choice ==2:
        
        choice_name = 'Paper'
        
    else: 
        choice == 3
        
        choice_name = 'Scissor'
        
    print("The User choice is: " + choice_name)
    print('\n')
    print("Now the computer's choice is: ")
    
    comp_choice = random.randint(1,3)
    
    if comp_choice == 1:
        comp_choice_name = 'Rock'
        
    elif comp_choice == 2:
        comp_choice_name = 'Paper'
        
    else:
        comp_choice==3
        comp_choice_name = 'Scissor'
        
    print('The Computer Choice is: ' + comp_choice_name)
    print('\n')
    print(choice_name + " V/S " + comp_choice_name )
    
    # Game tie Scenarios
    
    if ((choice == 1 and comp_choice == 1 ) or (choice == 2 and comp_choice == 2) or (choice == 3 and comp_choice == 3)):
        
        print('Its a tie!')
        
    # user winning scenarios
        
    elif ((choice == 1 and comp_choice == 3) or (choice == 2 and comp_choice == 1) or (choice == 3 and comp_choice == 2)):
    
        
        print(user_name + ' is the winner!')
        
    # Computer win Scenario
        
    else:
        ((choice == 2 and comp_choice == 1) or (choice == 2 and comp_choice == 3) or (choice == 3 and comp_choice == 1))
        
        print('Computer Wins!')
        
        
    print("Do you want to play further? \n (Y/N)")
    
    answer = input()
    
    if answer == 'N' or answer == 'n':
        break
        
        
  
    
        
        
