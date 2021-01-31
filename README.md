# Band-HackRU-Fall-2020
Band matches its users based on their Spotify history, specifically their top 10 most listened to artists. You can watch our demo video here: https://youtu.be/FhnM6oifTEg

Inspiration

Most dating apps geared towards young adults make it unnecessarily difficult to find others who share your interests-you could swipe through dozens of people before finding someone with a bio that piques your interest. Conversely, dating apps that match users based on interests often require lengthy profile setup. We believe it’s possible to solve both problems at once, which is why we created Band.

What it does

Band matches its users based on their Spotify history, specifically their top 10 most listened to artists. This not only gives matched users an excellent conversation starter, but is actually a good predictor of their chemistry as well. According to a worldwide study of 36,000 people conducted by a professor at Heriot-Watt University, music taste often correlates to other personality traits, meaning that users will have more in common with their matches than just music. Band also uses Spotify’s API to retrieve a user’s top artists. Our algorithm then parses this data and compares it with data from other users. While navigating through profiles, each prospective match is accompanied by a percentage indicating the proportion of artists the user has in common with said match.

How we built it

On the back end, we used Python to create a matching algorithm (and later translated it into Javascript to facilitate integration with our front end). Then we implemented the Spotify API to connect and authenticate users’ Spotify accounts, and to collect data on their top 10 most listened to artists. Following that, we used Angular to create the front end interface that allows users to login and register new accounts.

Challenges we ran into

Although we originally intended to use Datastax to store user profiles (including photos, bios, and song data), challenges with regard to integrating the database with our code resulted in us being unable to accomplish this in the given 24 hours. For demonstration purposes, we have inserted some data for sample users directly into our existing code.

Accomplishments that we're proud of

We're proud of Band's clean, intuitive user interface, and believe that it will facilitate the experience of using our application. We're also very pleased that we were able to successfully implement Spotify's API to connect and authenticate users' Spotify accounts.

What we learned

Kyle learned how to implement Spotify authentication in an Angular application, and more generally how authentication works. Erin C. learned how to use Angular, and about using documentation for Datastax and CWL inquiries. Erin M. created the matching algorithm and learned a lot about parsing JSON data in Python along the way.

What's next for Band

First, we want to improve our baseline functionality by integrating a database to store user profiles, allowing for more details on users to be stored, storing “swipes,” and alerting users of matches. We also would like to improve upon this baseline by creating messaging functionality, allowing for more sophisticated user filtering, and testing and improving our similarity algorithm. We also have some bigger dreams, like integrating the Spotify Search API into our messaging service so users can share songs, embedding playable music into profiles and bios, and showing users commonalities in music taste while viewing others. We will possibly run into some struggles with regard to scalability, ensuring user privacy, and runtime speed. Nonetheless, we are aware of the challenges and excited to face them head on!

Built With
angular.js
javascript
python
spotify
