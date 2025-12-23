Chat Site

This repository contains a lightweight web-based chat application built using Python and Flask. The project is designed to explore real-time messaging concepts, web development, and file handling while maintaining simplicity and clarity. It serves as both a learning exercise and a prototype for forum-style chat platforms.

Project Overview

The application allows users to interact through topic-based boards, create threads, and post messages with optional image attachments. Each board is dedicated to a specific topic, and users can browse boards alphabetically, search for threads, or engage in conversations by posting replies. Images are handled securely with file type validation and size limits, ensuring safe uploads to the server. The backend is lightweight and built entirely with Flask, utilizing standard Python libraries and minimal external dependencies.

Features

Users can view a list of boards, filter boards alphabetically, and navigate to specific boards to see threads. They can create new threads within any board by providing a title, and reply to existing threads with text content or image uploads. Uploaded images are validated against allowed file types and size limits and are stored in a structured uploads folder. For programmatic access, the application exposes an API endpoint to fetch posts in JSON format for a given thread. The backend includes robust error handling, including custom responses for invalid file uploads and oversized files.

Technical Implementation

The backend is implemented entirely in Python using Flask. Key components include routes for listing boards, creating and viewing threads, posting replies, handling image uploads, and returning post data as JSON. Image uploads are handled securely with unique filenames, and directories are created automatically if they do not exist. The server uses a simple in-memory data store (Python lists) for boards, threads, and posts to keep the prototype lightweight and easy to extend. This design allows clear visibility into the workflow of handling requests, storing messages, and managing file uploads without relying on external databases.

Design Philosophy

This project prioritizes simplicity, transparency, and educational value. By using only standard Python libraries and Flask, the implementation exposes the inner workings of a web-based chat system, including routing, request handling, data storage, and file management. It emphasizes readability, modularity, and minimal dependencies, making it an ideal resource for learning backend web development and experimenting with forum-style chat applications.

Future Directions

Planned improvements for this chat site include integrating persistent storage through a database such as SQLite or PostgreSQL, adding user authentication and permissions, implementing real-time updates with WebSockets, enabling richer media handling, and improving the frontend interface for better usability. The project can also be extended with moderation tools, search enhancements, and analytics to track activity across boards and threads.

Disclaimer

This project is experimental and educational in nature. It is intended for learning, prototyping, and personal projects rather than production use.
