# Event Storming for a Pinterest Application

![Alt text](<Pinterest Event Storming.jpg>)

---
## 1. Introduction

Event Storming is a collaborative domain modeling technique used to understand and design complex business processes. This report outlines the Event Storming process for developing a Pinterest application, focusing on key events, commands, and interactions within the system.

---
## 2. Domain Overview

A Pinterest application allows users to create, save, and organize images (Pins) into collections (Boards). Users can also interact with Pins through likes, comments, and searches, contributing to an engaging discovery-based social platform.
---
## 3. Key Domain Concepts

### 3.1 Entities and Aggregates

**User:** A registered account that interacts with the system by creating boards, saving pins, following other users, and engaging with content.

**Board:** A collection of pins that a user organizes by category or theme.

**Pin:** An image or video with metadata (description, link, and creator details) that can be saved to boards.

**Comment:** A user-generated message attached to a Pin.
---

## 4. Event Storming Breakdown

### 4.1 Identifying Key Events

Events represent significant state changes in the system. Below are the core events in the application:

#### User Events

`UserSignedUp`

`UserLoggedIn`

`UserUpdatedProfile`

`UserFollowedAnotherUser`

`UserUnfollowedAnotherUser`

#### Board Events

`BoardCreated`

`BoardNamed`

#### Pin Events

`PinCreated`

`PinSavedToBoard`

`PinEdited`

`PinDeleted`

`PinReported`

#### Interaction Events

`PinLiked`

`PinUnliked`

`CommentAddedToPin`

`CommentDeleted`

#### Search & Discovery Events

`UserSearchedForPins`

`UserViewedTrendingPins`

`UserDiscoveredNewPins`

### 4.2 Commands (User Actions Triggering Events)

Commands initiate state changes and result in events. Some key commands include:

`CreatePin`

`SavePinToBoard`

`FollowUser`

`PostCommentOnPin`

`LikePin`

`SearchPins`

### 4.3 Read Models (Views for End-Users)

**Board View:** Shows board details and its saved pins.

**Pin View:** Displays pin details, likes, comments, and related content.
---


## 6. External System Interactions

Image Processing Service: Handles image uploads and optimizations.

Search Engine: Supports search functionality for pins and boards.
---

## 7. Conclusion

Event Storming helps in designing a robust architecture for a Pinterest application by identifying key interactions, defining system boundaries, and modeling user behavior. This approach ensures that the system is scalable, user-friendly, and capable of delivering an engaging experience.