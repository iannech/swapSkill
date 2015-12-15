# swapSkill
Android app 

# About
Swap lets users do each other's task and exchange stuff in a fun way. 
Users can do each other's assignments or carry out physical tasks on behalf of other people.
Users in one location can exchange Games, Movies plus more..

# Profile Set up
##Signing Up
Swap uses oped id signup service from facebook. Users can therefore sign up via facebook.

## Why sign up?
Signing up allows users to - Add skills (for easy filtering of tasks).
                           - Add Items to the Swap Inventory (These are items they want to exchange).
                           
## Adding Skills
A checklist of skills is provided for user to check as much as possible. An "other" button exists for manual entry of skills not featured in the list. These are saved to user profile.
## Adding Item
An "Add" button exists in the inventory. Tapping the button allows user to add new item for exchange. Parameters [Image of item, Name, Some description]. These are saved as user data on the cloud. A cache of the media files can be made on local storage of the user.
## Editing profile
User can edit their profile any time. 

# Handshake
A "handshake" is the binding feature in the app. 
From a list of available Tasks, a user can "TAP" on one -> to open an activity with more info about the task -> At the bottom is a handshake icon which the user taps to send handshake(this means a person is ready to do the task)-> Task owner receives a handshake request notification -> Tapping back means they've accepted to have their task done by the first user -> The two users will then exchange contacts (email address + phone number should do). 

# Leader Board
Ranks the people who have completed the most tasks. Design issues: location aware or not?

# Target 
Students are the primary target but everyone is free to use.
Once profile is complete, they'll fill in all the skills they possess and wanna share with world.
Users can add items they wish to exchange to their inventory . 

Once a user has completed their profile setup, they immediately gain access to the swapSkill platform:-
	- They can see tasks/assignments that people in their location want done
	- They can see items for exchange around their location.
	- They can search for a particular Skill and see a listing of all the people with the same skill.
	- They can Search for people - Trying to access people's profile is only possible if they are around your location(not sure of this yet).
	- Shake hands to do a task/request an exchange of an item.
	- Accept a Handshake for someone to do your task/exchange item . 
# Requirements
	1. User login(Oauth) - Facebook, Twitter.[AMAZON COGNITO]
	2. Store and sync user data - user details, item images, profile pics[AMAZON S3]
	3. Backend logic[AWS LAMBDA].
	4. Location aware - show tasks around user location ?? - not a must
	5. Push notification - app send notification to all users[AMAZON SNS]

