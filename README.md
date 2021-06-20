<h1>MissingPeople </h1>

### Inspiration

I searched for the websites that post the cases of missing person. People have to click a lot to view the information for each cases. Therefore, I create a website that only ask the user to input the information of the cases and user can look at other cases at the bottom of the page.

### What it does

It allows people to report the missing cases and check the other cases. Once the user submit the case profile, it will be added to the database and display on the website right away after the user click the button to refresh the page. User can update the profile information or even delete the profile once the person is found. Select Image button: ask user to select any image from their local device Upload Image button: upload the image of the current profile to the database

### How we built it

For the backend, I use Firebase tools such as Firestore Database, Realtime Database, Cloud Storage and Hosting. Firestore Database stores the missing person's data such as name, age, gender, date of birth, weight, eyes, hair, height, build, race, scars and marks, last seen, details, contact. The Cloud Storage stores the images. Realtime Database stores the name of the missing person and the image link from Cloud Storage. I use Firebase Hosting to deploy and host the website. For the frontend, I use HTML and CSS.

### Challenges we ran into

- Getting the list of data from the database and display on the website
- Retrieving the list of images from Cloud Storage Since I use different database to contain different information, I have to use different calling method to get/write - the data. For example, firebase.storage().ref('someString').otherMethod and firebase.database.ref('someString').otherMethod.

### Accomplishments that we're proud of

I would love to continue to work on this project because I believe it can be used in a good way in the future so I would like to add some more features such as allowing user find cases at specific location, using the google maps to find the local police station, sort the cases by locations and solved or unsolved cases. I'm proud that the website works!

### What we learned

This is the first time I use most of the tools in Firebase

- Learned how to insert/select/delete/update user's data
- Learned how to upload and retrieve images from Cloud Storage
- Learned how to delete the user's profile by deleting user's data from Realtime Database, Cloud Storage and Firestore Database.

### What's next for MissingPeople

- Add the google map that pins the location of police stations
- Allow user to find specific cases at specific location

### Link
- https://devpost.com/software/missingpeople
