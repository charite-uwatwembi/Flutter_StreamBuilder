

# Simple Chat App with StreamBuilder

## Overview

This is a basic chat application built with Flutter, showcasing the use of the `StreamBuilder` widget for real-time updates in the UI. Users can input messages which are instantly displayed in a chat interface.

## Technologies Used

- **Flutter**: A UI toolkit for building natively compiled applications for mobile, web, and desktop from a single codebase.
- **StreamBuilder**: A Flutter widget that rebuilds itself based on the latest snapshot of interaction with a `Stream`.

## How It Works

### Main Entry Point

The app begins with the `main` function which initializes the `MyApp` widget using `runApp`.

### MyApp Widget

- Root of the application structure.
- Uses `MaterialApp` to set up the app's basic theme and structure.
- `debugShowCheckedModeBanner` is set to `false` to remove the debug banner.
- Includes an `AppBar` and `ChatScreen` as the main body widget.

### ChatScreen Widget

- `StatefulWidget` managing the state of chat messages.
- Utilizes a `StreamController` to handle and emit a stream of messages.
- `StreamBuilder` listens to this stream and updates the UI in real-time when new messages are added.

### MessageInput Widget

- Manages user input for sending messages.
- Contains a `TextField` for entering messages and an `IconButton` to submit them.
- Sends the entered message to the `StreamController` when the send button is pressed and clears the input field.

## Code Structure

- **main.dart**: Contains the entire application code.
  - **MyApp**: Sets up the main structure and theme of the app.
  - **ChatScreen**: Manages the chat interface and handles real-time message updates using `StreamBuilder`.
  - **MessageInput**: Handles user input and message submission.

## Functionality

- Users can input messages which are added to a list managed by a `StreamController`.
- The `StreamBuilder` widget listens to this list and updates the chat interface in real-time with new messages.
- Simple and intuitive user interface for sending and displaying messages.

## Presentation Highlights

- Illustrates the use of `StreamBuilder` for dynamic UI updates.
- Modular code structure with separate widgets for different app functionalities.
- Ideal for learning Flutter's real-time data handling capabilities and building interactive application.
