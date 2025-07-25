# EnrollNow

I wanted to enroll all device at my organization without wiping. This is possible by registering the devices to DEP via your Apple Dealer. You are then able to assign the devies to a PreStage enrollment.
The enrollment will happen at some point then and you can trigger it with "sudo profiles renew enrollment" or "sudo profiles -N". I wanted my user to be informed via E-Mail but I didn't want them to wait 
for the enrollment happen automatically and I didn't want them to have to open the Terminal and enter the command. Therefore I created this small app. "launchctl asuser" was the only way to get this to work

Just executing the script or using osascript do shell script didn't work and gave me an "DEP enrollment (null) error"

You can send this Small app via e.g. E-Mail to your users after you selected an already setup device in Jamf Pro in a PreStage enrollment. The app practically triggers "profiles -N" to start the enrollment process.

## Sign and notarize the app before use otherwise the user has manually approve everything :(

1. Select an already setup device in jamf pro (no wipe required!)

<img width="2171" height="344" alt="Screenshot 2025-07-25 at 15 18 56" src="https://github.com/user-attachments/assets/2103b6c4-40cb-4563-9d01-6cde700a8fca" />

2. Send them the app. User can double click and enrol, see the gif attached

![Untitled](https://github.com/user-attachments/assets/c27ac808-6c1e-407a-865e-0d0740fed71d)
