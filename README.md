# CS-360-Mobile-Arcitecture-and-Programming

**Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?**

The app I developed is called WeighArc. It was designed to give users a simple way to track their weight, save a goal weight, and see changes over time. 
The main requirements included account creation and login, storing weight data in a SQLite database, allowing users to add, edit, and delete weight entries, and supporting SMS notifications when a goal weight is reached. 
I wanted the app to be easy to use without adding features that would make it feel complicated.


**What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?**

The app needed a login screen, a weight history screen, and an SMS notification settings screen. The login screen lets users create an account and sign in. 
The weight history screen shows saved weights in a table and includes controls for adding, editing, and deleting entries, along with setting a goal weight. 
The SMS screen lets the user enter a phone number and turn notifications on or off.

I tried to keep the screens simple and make the main controls easy to find. I also used color coding so a weight loss appears in green, a gain appears in red, and no change appears in black.
The newest weight is shown at the top of the list so users do not have to search for it. I think the design was successful because the main features are easy to reach and the app does not require the user to move through unnecessary screens.


**How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?**

I worked on the app in smaller pieces instead of trying to build everything at once. I started with the screens and navigation, then added the database, login features, weight management, goal weight, and SMS notifications. 
I tested each part before moving on to the next one.

I also used separate methods for different tasks, such as adding weights, updating weights, loading saved data, and checking whether the goal weight had been reached. 
This made the code easier to follow and made it easier to find problems when something did not work. I could use the same approach in future projects by breaking larger features into smaller parts and testing them as I go.

**How did you test to ensure your code was functional? Why is this process important, and what did it reveal?**

I tested the app in the Android emulator throughout development. I tested creating an account, using a correct and incorrect password, logging out, adding weight entries, editing them, deleting them, and checking that the data stayed saved after leaving the screen. 
I also tested the goal weight and SMS settings, including what happened when SMS permission was granted or denied.


**Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?**

One challenge was displaying the weight history while still keeping the controls on the screen usable. As more entries were added, the table could take up too much space. 
I changed the layout so the weight history could scroll while the controls for adding weight, setting a goal, logging out, and opening SMS settings stayed available.

Another challenge was the color coding. The app needed to compare each weight with the previous entry so it could determine whether the user gained weight, lost weight, or stayed the same. 
I changed how the database results were read so the comparison could be done in the correct order while still showing the newest entry at the top of the screen.


**In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?**

I think the weight history and database features were the strongest part of the app. 
The app can save real weight entries in SQLite and allows the user to add, view, edit, and delete them. I also connected the saved data to the UI instead of using hardcoded sample information.

The color coding, goal tracking, and SMS notification feature also work with the saved data. 
That part of the project showed that I could connect the user interface, database, and application logic together instead of treating them as separate pieces.
