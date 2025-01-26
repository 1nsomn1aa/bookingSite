
![Image](https://github.com/user-attachments/assets/febec2af-80f0-4ce6-a0fe-8f232da18304)


**Dundalk Stadium** is a website for a stadium in Dundalk. The site allows users to find information about the latest news, events, current facilities, history, opening times and other relevant information. Users can create an account and check bookings for their desired courts, by checking if their selected time and day is available on our database.


[Link to Dundalk Stadium on Heroku](https://dundalkstadium1-872936dbe739.herokuapp.com/)

## Features

**Design**

The design choices on this project were selected with simplicity in mind. The project uses bright and colourful pictures, because of that, it was decided to mainly use only Black & White colors with adjustments to their brightness or opacity. The end result looks clean, without too many unwanted distractions. 

![Image](https://github.com/user-attachments/assets/1fe9eaa0-e23f-482f-a6e5-e5a765d76a94)

**Typography**

The font used on the main page is mainly "Playfair Display", due to having the old newsletter look, which reminds people of the old heritage of the stadium. Other pages used default Bootstrap fonts, to showcase modern features like bookings, contact form and profile page.

![Image](https://github.com/user-attachments/assets/45aecf8d-df3b-4893-980c-7fd1509585aa)

**Landing Page**

The landing page shows an aerial picture of the Dundalk Stadium. The header/navigation bar is fixed to the top and has lower opacity to allow some visibility of the page, without making it hard to read the text. The center of the screen displays a brief description of what is Dundalk Stadium and showcases the most used links to help users navigate to the most popular areas of the site.

In mobile view the navigation bar turns into a dropdown menu, saving on valuable screen space and ensuring that the links are easier to press on a small screen.

*Desktop Version*

![Image](https://github.com/user-attachments/assets/c0437e07-de2c-4df4-a994-2da80d7acb95)

*Mobile Version*

![Image](https://github.com/user-attachments/assets/c6ef0fb5-b69b-4bf6-ae52-c004637a1aee)

**Events Page**

The events page is a simple page that displays the name, date, time, price, loctaion and a short description of our upcoming events. Behind the information div, there is a background picture generated by AI which corresponds specifically to the event.

*Desktop Version*

![Image](https://github.com/user-attachments/assets/b2abf210-44c4-43f2-ae35-24e8af712beb)

*Mobile Version*

![Image](https://github.com/user-attachments/assets/8ce1dcc0-57ec-47b2-8533-19c98be52010)

**Booking Page**

Booking page showcases a few selections: Game Type, Court and Date. Registered users can select their desired game, court and date and press "Check Availability". This collects users information and checks for available times in our database. The page reloads, showing the users selection and the available times. By selecting the time and pressing "Book Now" the user will save the booking to their user account and will get redirected to the profile page with a message "Booking successful".

*Desktop Version*

![Image](https://github.com/user-attachments/assets/4a2180f8-18a8-4311-ab7f-fc95db3083b9)

*Mobile Version*

![Image](https://github.com/user-attachments/assets/3e7c1f89-5002-484e-9d8c-50f64a0a3b5a)

*Game Type Selection*

![Image](https://github.com/user-attachments/assets/94072768-3554-40b8-8ca4-a7eaa0cc6db6)

*Court Selection*

![Image](https://github.com/user-attachments/assets/5419e581-7a0d-4a39-9571-76fd44818537)

*Returned Results*

![Image](https://github.com/user-attachments/assets/d39eec4b-67c5-4263-86e2-0f6a33b75256)

**About Page**

The about page displays to the users a brief history and the most interesting facts about the Dundalk Stadium.

*Desktop Version*

![Image](https://github.com/user-attachments/assets/dadbb0cc-e0fd-462e-9861-cafa3961c824)

*Mobile Version*

![Image](https://github.com/user-attachments/assets/15332f5c-e951-4f76-96f4-74be78943996)

**Contact Page**

The contact page allows users to quickly reach out to the administrators of the page by filling out a simple form with their First and Last Names, E-Mail address, Topic and their message. The form includes validation checks before sending the data out. If the validations pass, the message is sent and an alert is displayed "Your message has been sent successfully. We will get back to you soon!".

*Desktop Version*

![Image](https://github.com/user-attachments/assets/6028d11d-9f3a-4603-ac57-749425282347)

*Mobile Version*

![Image](https://github.com/user-attachments/assets/1895a040-3026-499f-a2f1-a1d1f8488459)

**Profile Page**

The profile page can only be accessed by registered users, if the user tries to enter the profile page manually by typing in the profile page url, they will be redirected to the login page. On the profile page, users can edit their Username, Email and upload an image.

If the user uploads an image that is bigger than 300px (width or height) the view logic will automatically resize it to be 300px x 300px. The image uploads are handled by Amazons AWS S3 and IAM services. 

At the bottom of the profile page, there is a section for the users current bookings. The section searches our database to find entries for the associated user account and any of their bookings and displays them here. Users are also able to delete the bookings from our database, making that booking available to someone else.

*Desktop Version*

![Image](https://github.com/user-attachments/assets/b0f548fd-6d42-4ed9-b3e0-61783fa97dbe)

*Mobile Version*

![Image](https://github.com/user-attachments/assets/b0cbdede-ca3c-452e-8cd1-cb1beb75bdbb)

*Bookings*

![Image](https://github.com/user-attachments/assets/b2303ada-ab25-440b-b138-06a875f8fdc3)

**Login / Logout / Signup / Password Reset Pages**

The user accessibility pages were created to allow users to create accounts in order to access restricted areas on the website. The password reset page was also implemented in order to allow the users to reset their password on their own, without having to contact the administrator.

*Logout*

![Image](https://github.com/user-attachments/assets/3f3cef46-7f8b-4985-88d3-b33d931eb9b6)

*Login*

![Image](https://github.com/user-attachments/assets/8488111f-9415-4bf0-aaad-3e932f7d37ca)

*Sign Up*

![Image](https://github.com/user-attachments/assets/d575d793-ad2b-40a0-b4a3-996a2e6e362f)

*Password Reset*

![Image](https://github.com/user-attachments/assets/31768972-ddc4-4a60-9a5a-0ff966dcd2f2)

**Administrator Page**

The administrator page allows users with staff or super user privileges to create, edit or delete content on the website:

- Create, delete or edit the information about Users or make Groups for multiple users with the same class.
- Bookings tab enables administrators to quickly check current bookings, edit, delete or create new ones for a specific user. They are also able to create new types of games or add new courts.
- The news section allows administrators to create, edit or delete Latest News bulletins on the page. They can also assign them to specific users.
- At the bottom page there is a recent action log provided by django, that showcases the most recent actions taken by specific users.

*Mobile View of the Admin Panel*

![Image](https://github.com/user-attachments/assets/67d7e09b-ece9-4e74-b7fb-87f90bb12efb)

**Custom Error Handling**

If a user tries to navigate to a page that does't exist, they will be redirected to a code 404 error page, which will inform them that the page they are looking for doesn't exist and suggest them to return to the home page.

In a case when there is a problem with our site, the webpage displays a code 500 error, informing the users that there is an interal problem with our servers.

*404 Desktop View*

![Image](https://github.com/user-attachments/assets/0828b969-6b5d-400f-af27-1cfd0b1de7eb)

*500 Desktop View*

![Image](https://github.com/user-attachments/assets/523be6ea-7213-4f7f-b17f-7b4cb54e47ba)

## Agile Development

I used GitHub Projects as an Agile tool for this project. By setting up specific templates for user stories and epics, together with their accompanying tags, I was able to prioritize my development and rethink what features were necessary using the MoSCoW method.

Tasks, issues, and user stories were tracked weekly using the GitHub Projects board.

*GitHub Project Board*

![Image](https://github.com/user-attachments/assets/7f865fd6-abb4-40df-94b9-b9bc70915d66)

*GitHub Issues: Epics and User Stories*

![Image](https://github.com/user-attachments/assets/e897431f-0be8-4423-aaaf-34ebd11949a3)

## Testing

For all our testing, please refer to the [TESTING.md](https://github.com/1nsomn1aa/DundalkStadium/blob/main/TESTING.md) file.

## Bugs

During the development of this project, I've encountered some bugs:

- The deployed website wouldn't work on heroku, giving me error codes for the inability to spawn workers. I managed to fix this issue by deleting an extra space in my Procfile.

- The page wouldn't serve media files from Amazon AWS. This was resolved by adding a few lines to my settings.py file about the region used for amazon aws and its version.

- At the begining of this project, I encountered many bugs due to improper linking of my views to my urls. All of these issues were resolved by reading the Code Institute LMS and watching tutorials on YouTube.

To my knowledge, there are currently no bugs on this website and everything works as it should.

To see my development process and bug fixes, please follow [this](https://github.com/1nsomn1aa/DundalkStadium/commits/main/) link to my GitHub repository.

## Deployment

This website has been deployed to Heroku. The steps I took to do this are outlined below. 

- [x]   Create a Heroku Account
- [x]   Sign up at Heroku if you don’t already have an account.
- [x]   Install the Heroku CLI (Optional)
- [x]   Download and install the Heroku Command Line Interface (CLI) from Heroku CLI for additional control if needed.
- [x]   Create a New Heroku App
- [x]   Log in to your Heroku dashboard.
- [x]   Click the “New” button, then select “Create New App.”
- [x]   Enter an app name (unique across Heroku) and choose your region.
- [x]   Connect Heroku to Your GitHub Repository
- [x]    Navigate to the Deploy tab in your Heroku app dashboard.
- [x]   Under Deployment Method, select GitHub.
- [x]   Authorize Heroku to access your GitHub account, if prompted.
- [x]   Search for and select your GitHub repository.
- [x]   Enable Automatic Deploys (Optional)
- [x]   In the Automatic Deploys section, click Enable Automatic Deploys if you want Heroku to deploy every time you push changes to the main branch.
- [x]   Deploy Your App
- [x]   To deploy manually, scroll down to the Manual Deploy section.
- [x]   Select the branch you want to deploy from (e.g., main) and click Deploy Branch.
- [x]   Check Your App
- [x]   Once deployed, click Open App at the top-right corner of the dashboard to view your app live.
- [x]   Set Environment Variables (Optional)
- [x]   If your app requires environment variables (e.g., API keys), go to the Settings tab in Heroku.
- [x]   Click Reveal Config Vars and add your variables in the form of key-value pairs.

## Credits

**Images**
- Logo has been created using Photoshop.
- All content related pictures were generated using [Ideogram AI](https://www.ideogram.ai)
- Default profile picture was taken from [freepik](https://www.freepik.com) .

**Other Resources**

- HTML/CSS/JS/PYTHON questions [W3Schools](https://www.w3schools.com/), [freecodecamp](https://freecodecamp.org/) and my previous [GitHub Projects](https://1nsomn1aa.github.io/)
- Django Project Set-Up [YouTube](https://www.youtube.com/channel/UCCezIgC97PvUuR4_gbFUs5g)
- Icons [FontAwesome](https://www.fontawesome.com/)
- Fonts [GoogleFonts](https://www.fonts.google.com/)
- Code Editor [GitPod](https://gitpod.io/)
- Cloud Storage [GitHub](https://github.com/)
- Deployment [Heroku](https://www.heroku.com/)
- Validation [W3C HTML](https://validator.w3.org/), [W3C CSS](https://jigsaw.w3.org/css-validator/) and [JSHint](https://jshint.com/).