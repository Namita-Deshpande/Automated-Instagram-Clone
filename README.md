Instagram Clone SQL Project

Overview:
This SQL schema is designed for an Instagram clone application. It aims to provide a robust and scalable database structure to handle user data, posts, likes, comments, and follows. The schema is relational, optimized for performance and designed to ensure data integrity and support complex queries.

Features:
Users Table: Stores user information including username, email, password (hashed), profile picture, bio, and other personal details. Each user has a unique ID.
Posts Table: Contains details about posts such as the user ID of the poster, image/video URLs, caption, location data, and timestamps.
Comments Table: Holds comments made on posts. Each comment is linked to a user and a post, along with the comment text and timestamp.
Likes Table: Records likes on posts. It relates the user who liked and the post that was liked.
Follows Table: Manages the following relationships between users, indicating who follows whom.
Stories Table: Manages short-lived stories posted by users, with references to the user and media content.
Direct Messages Table: Facilitates private messaging between users, storing the sender, receiver, message content, and timestamps.
Relationships:
Users have a one-to-many relationship with Posts, Comments, Likes, and Messages.
Posts have a one-to-many relationship with Comments and Likes.
The Follows table has a many-to-many relationship between users, indicating followers and followees.
Security and Performance:
Passwords are stored securely using hashing algorithms.
Indexes are used for frequently queried columns to speed up searches.
Foreign keys enforce referential integrity between tables.
Scalability:
The schema is designed to handle large numbers of users and activities efficiently.
Considerations for future scaling include partitioning tables and optimizing queries.
Getting Started:
Clone the repository.
Use the provided SQL files to create your database schema.
Adjust and extend the schema as needed for additional features or custom functionality.
Contribution:
Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.
