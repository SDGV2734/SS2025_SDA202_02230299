# Glossary of Domain terms 

![alt text](<Blank Diagram from Lucidchart.png>)

- **User**:
  - Represents an individual using the app, having attributes like username, email, password, and profile details.
  
- **Board**:
  - A collection of Pins organized by a user. Users can create multiple boards to group their saved Pins.

- **Pin**:
  - An image or post that a user can "pin" to a board. It includes metadata like the image URL, title, description, and tags.

- **Upload**:
  - A record of an image uploaded by a user, which can later become a Pin. Contains metadata such as the image URL and upload status.

- **Notification**:
  - A message or alert sent to a user, often indicating actions like new followers, likes on Pins, etc.


- **PinImage (Value Object)**:
  - A value object associated with a Pin that contains metadata related to the image, such as its resolution or format.

- **Authentication**:
  - The process of verifying a user's identity when they log in, often involving username/password verification.

- **User Profile**:
  - Contains personal information about a user, such as their avatar, bio, and other settings.



- **Upload Status**:
  - Indicates the state of an image being uploaded, such as "pending," "successful," or "failed."


- **Aggregate**:
  - A cluster of domain objects treated as a single unit. For example, a `Board` and its associated `Pins` can be considered an aggregate.

- **Value Object**:
  - An object that holds attributes but has no identity. Examples include the `PinImage` value object, which contains metadata but doesn’t have its own identity apart from the Pin.


