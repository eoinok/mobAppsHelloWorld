# Step 1 - Create a React Native Expo "Snack"
Open the website Expo.io Register a new account.
Create a new "Snack" 
Click on the "i" information small icon at the top of the page and Edit Details. Change the Project Name to helloWorld and the description to "My First React Native App"
Then Change the Starter code and replace it with the simpler code shown below.
![image](https://github.com/user-attachments/assets/ce887abc-c2ed-424a-946a-46e366be99b1)

Once your code displays correctly on the screen on the right -
Download the "Expo Go" App from either the Play Store or App Store to your phone

![image](https://github.com/user-attachments/assets/9523b122-a27f-4e9d-b77b-9b87b1615dc8) ![image](https://github.com/user-attachments/assets/d8e9e88b-7cf1-4fe4-8f30-4b8cef796117)

click the "My Device" button
Follow the QR Code
This should open the Expo Go app on your Phone and load the Snack.
The App will not look good and the some of the Hello World text may be obscured in the top left hand corner of the screen but we can fix these issues as we go forward. You've created your first phone app - kindof.

Export the code to a zip file. Add these files to your repo and commit the code.

# Step 2 - Add a style to the Text
Add the following code below the import statement
```
const styles = StyleSheet.create({
  paragraph: {
    margin: 24,
    fontSize: 18,
    fontWeight: 'bold',
    textAlign: 'center',
  },
});
```
This creates a variable called styles. On the right side of the equals a StyleSheet object is being instantianted. It is being passed a JSON array containing settings as an argument. To use this stylesheet you must add "StyleSheet" to the list of react native components beging imported on the first line.

In order to add this style to our Text component we must pass it to the component as a prop. Look up how to add a prop to a component on w3schools - react. Bare in mind that the style is a variable so you must refer to it using braces - i.e. {styles.paragraph} when you've managed to change your App so that the text appears differently add this new code to the file you committed in Step 1. Commit and push your new code as Step 2

# Step 3
Add in the following line at the top with the other import statement
```
import React, {useState} from 'react';
```
This will allow us to use the useState "hook"
Set up and array variable in which to store the value for the useState hook by adding the following line - use your own name.
```
const [fullname, setFullname] = useState("Eoin OKennedy");
```
Add this variable in beside your Hello World inside the text component (hint - you must enclose it in braces for the component to recognise it as a variable)
When you get your name to display beside the Hello, World add the new code to your repo and then commit and push your code.

# Step 4
Try and lookup how a TextInput component works. Try and add one to your app. Try to use the onChangeText prop of the TextInput component to call the setFullname() method passing the value of the text entered by the user. This should change the display to read Hello, World, Jimmy (if "Jimmy" was entered by the user.


