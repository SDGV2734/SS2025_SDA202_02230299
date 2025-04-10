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

- **FeedItem**:
  - A wrapper for Pins displayed in a user’s feed, often ranked by relevance score.

- **PinImage (Value Object)**:
  - A value object associated with a Pin that contains metadata related to the image, such as its resolution or format.

- **Authentication**:
  - The process of verifying a user's identity when they log in, often involving username/password verification.

- **User Profile**:
  - Contains personal information about a user, such as their avatar, bio, and other settings.

- **Tags**:
  - Keywords associated with Pins to make them easier to search for or categorize.

- **Relevance Score**:
  - A metric used to determine how relevant a Pin is to a user, often based on user behavior, interactions, or preferences.

- **Upload Status**:
  - Indicates the state of an image being uploaded, such as "pending," "successful," or "failed."

- **Multiplicity**:
  - The cardinality of relationships between entities, typically expressed as 1-to-many, many-to-one, etc.

- **Aggregate**:
  - A cluster of domain objects treated as a single unit. For example, a `Board` and its associated `Pins` can be considered an aggregate.

- **Value Object**:
  - An object that holds attributes but has no identity. Examples include the `PinImage` value object, which contains metadata but doesn’t have its own identity apart from the Pin.

- **Service**:
  - A domain service contains business logic that doesn’t naturally fit within an entity or value object, such as the `PinService` for creating, deleting, and managing Pins.

- **Context**:
  - A boundary around a set of related concepts in a domain. For example, the `UserContext` encapsulates everything related to users, while the `BoardContext` handles boards and pins.
