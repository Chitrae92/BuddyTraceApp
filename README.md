# BuddyTraceApp
The Buddy Trace App is used for tracking friends and family all over the world in real-time. It enables users to pinpoint the location of people that they are in a group with.
  
## Sign Up
On opening the app, a splash screen appears which lasts for 2 seconds followed by the introduction screen for the app. When the “get started” button is clicked, a signup page is displayed where users can enter their phone number for login. Once a valid phone number is entered, the Firebase backend database automatically sends an SMS with a 6 digit verification code to the entered phone number. If the verification code matches, the user will be successfully logged into the app. Otherwise it throws an error as "invalid code". 

![Alt Text](https://github.com/Chitrae92/BuddyTraceApp/blob/master/Flash%20Screen.PNG)

![Alt Text](https://github.com/Chitrae92/BuddyTraceApp/blob/master/SignUp.PNG)

  
## Maps API and features
Upon successful login, the profile page is displayed and asks the user to input a display name. Once saved, the user is redirected to the map home screen. The Google Maps API appears with the marker showing the user's current location as well as different markers locating everyone in the group that the user is in. On the map home screen, users can click a dropdown menu on the top right corner to select which group they want displayed on their map. The map also has a button to center on the user’s current location in case he or she scrolls too far away. The user can click the navigation drawer icon on the top left of the screen, or swipe left, to navigate to the groups, friends, and profile screens. From the menu screen, clicking on groups takes you to the groups list screen which displays the current groups the user belongs to and clicking the add button at the bottom allows the user to create new group. An edit page will display for creating new group which asks users to enter necessary information including group name, description, and destination. Group members should then be selected from the user’s friend list on the app. The group will be saved in Firebase and added in group list after user click save button.

![Alt Text](https://github.com/Chitrae92/BuddyTraceApp/blob/master/HomeScreen.PNG)

### Creating groups
New groups without members or without the necessary information are not allowed and will display a message on screen reminding users to enter in that information. When a new group has been created successfully, users can selected that group from the map screen to trace the location of all the members in that group. Users are able to see the details of a group by clicking on the group on the group list page, and they will be navigated to group detail page showing all the information about the group and existing members. The delete button on the group detail page is used for deleting the whole group,an alert dialog will display to confirm deleting. Once a user deletes that group, the data will be deleted from Firebase and disappear from all group members’ groups list. 

![Alt Text](https://github.com/Chitrae92/BuddyTraceApp/blob/master/Groups.PNG)

### Adding friends
Users can also add friends from which they can create groups with and add to groups. Friends are located from a user’s contact list on the phone. Any contacts that are in our Firebase database will be available to add as friends, any contacts not in our database can be invited to join the app.
