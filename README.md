![](http://i.imgur.com/ccLUqLU.png)

# Code Challenges

Our main goals:
* Simulate a code challenge you might receive from an iOS employer.
* Sharpen your iOS/Swift knowledge by challenging you to learn new topics.
* Make Barry happy.

This is a project that you should work on _alone_. Where pair-programming is great, the following challenges are meant to simulate code challenges you would submit to an employer that you would have worked on by yourself. The instructions are meant to be vague. Focus on the most important parts of making it work--but make sure it's code you would be proud to show someone. If there are any questions as to the direction of where you should go, feel free to message us on Slack. As to answering _specific_ questions to the code you will be writing, realize that we won't be giving you a direct answer which would solve your problem. We might point you in the right direction or steer the ship away from crashing into an ice-berg (.. never let go Jack), but realize that this is for your benefit.


# Magic: The Gathering (Advanced)

![](http://i.imgur.com/t2gDkTQ.jpg)

Create an iOS application that allows the user to interact with the [Magic: The Gathering API](http://docs.magicthegathering.io/#overview).

### Specifications

* A user should be able to search for Magic: The Gathering cards to then view them in a `UICollectionView`.
* A user should be able to view all Magic: The Gathering cards in a `UICollectionView`. Use the `page` url parameter to view more results. You can also adjust the limit via the `pageSize` url parameter. This has a maximum of 100 cards per request.
* A user should be able to tap on a cell and see a detail view with information about the card.
* If the card is **Rare** or **Mythic Rare** then the cell and detail view should indicate that in some way.
* All search results should be persisted in a Realm database.
* Please use the Realm `Results` collection type as the collection view's data source.


### Libraries

You should use CocoaPods to install Realm, and you may use other 3rd party libraries **except** for network requests and parsing JSON.


### Architecture and Testing

Use MVVM as it helps _de-bloat_ ViewControllers and improves testability. You don't need to be an expert in MVVM but you should follow the basic principles.