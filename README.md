# TraceCovidSenegal
## Splash Screen While Loading Components 
    With Explanations and Next Button 
    This Screen will have some explanations about the 
    app to distract the user while the app is 
    loading on background
    Once the loading is complete, the Next Button becomes enabled  
## First Connexion 
###  Ask for PERMISSIONS 
        * bluetooth activation permission
        * running on background permission
        If accept
          Active bluetooth
          Active Background Task Running
          Show Login View
        Else 
          Quit with message 
### Authentication on First Connexion with permissions
      Show input, user is prompted to enter his phone number
      Send a one-time code and Verify validity
      Create a new user instance on Firebase (User: uniqueID, phoneNumber, createdAt)
      Generate a daily temp ID from uniqueID
      Send back to user (tempID, createdAt, expiresAt)
      Save locally on asyncStorage
## On every App Opening 
      Main View | Alert View | Help View | ..
    
##    On Background 
      Periodic Blutooth Advertisement
      Periodic Bluetooth Scan
      If a device is found 
        Get Device's tempID    
      
##  Every Day 
      Generate a new tempID from uniqueID
    
    If declared positive
      Receive message from Health Authority
      Prompted to share our contact list with contenment
      Publish Contact List
      Broadcast Message to every contact from saved phone numbers
      Broadcast Message to every contact of contacts from saved phone numbers
      Create a groupe of peopleToQuarantine
