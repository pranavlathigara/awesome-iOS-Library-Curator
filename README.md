# iOS_Library_Curator
A review of each project I "Star" On Github. 

As you can tell from my profile, I "STAR" more projects than prety much anyone else. This document is an attempt to break down ech and every one of these! Feel free to contribute! Note: I primarily use Obj-C and this list clearly reflects that. I will make a seperate list for Swift projects

## **iOS List**

Here's how this list is going to be categorized:
- Essential Projects
- ReactiveCocoa Extensions
- Library and Frameworks
- Plugins
- Good Websites
- My Personal Favorites
- Example Projects (to be broken down furthur)

#### First, the gold standard libraries. The essentials --- You **NEED** to know about these !! You're likely to include each of these in most of them

- **AFNetworking**: Probably the most "starred" iOS project on Github, and for good reason. AFNetworking wraps most of the complicated NSURLSession / HTTP / Core Data into one easy to use library.
- **ReactiveCocoa**: If you haven't heard about this one, well, you're in for a serious treat. This lib makes your iOS code _Functional_ and _Reactive_.
- **Mantle**: A great lib for creating Model objects in iOS. Normally, this requires a ton of boilerplate code. Now, it doesn't have to!
- **RESTKit**: A fantastic library for making REST type requests in iOS with WEB services relatively painless. It provides a powerful object mapping engine that seamlessly integrates with Core Data and a simple set of networking primitives for mapping HTTP requests and responses built on top of AFNetworking. It has an elegant, carefully designed set of APIs that make accessing and modeling RESTful resources feel almost magical.
- **Masonry**: You got autolayout issues? Don't like using storyboards? Hate autolyout code? (I know I do!) Use this library instead! 
- **Objection**: Dependency Injection in objective-c made sooo much easier with this. A great great lib
- **Specta**: A light-weight TDD / BDD framework for Objective-C & Cocoa. This makes testing your code a piece of cake
- **Expecta**: A matcher framework that works fantastically with Specta. expect(**expecta**).to.beAwesome() for testing your ReactiveCocoa code

#### Next, because ReactiveCocoa should transform EVERYTHING when it comes to writing iOS code, here's a few extensions that should make your RAC transtion a little bit smoother

- **Firebase + RACExtensions** (my own)
- **ReactiveCocoaLayout**
- **ReactiveViewModel**
- **ReactiveCoreData**: Below is an example of how this lub can be used
            RAC(self.filteredParents) = [[[[Parent findAll]
              where:@"name" contains:filterText options:@"cd"]
              sortBy:@"name"]
              fetchWithTrigger:objectsChanged];
- **CETableViewBinding**
- **Bikes**


####Library and Frameworks
- Audio
- Cache
- Core Data
- Charts
- Database
- HUD
- iBeacon
- Images
- EventBus
- JSON
- Layout
- Logging
- Maps
- Location
- Networking
- Push Notifications
- Passbook
- Text
- Walkthrough / Intro / Tutorial
- UI
- Websocket
- Code Quality
- Analytics
- Payments
- Products
- Utility
- Security
- Video
- Project setup
- Dependency / Package Manager
- Testing
- TDD / BDD
- UI Testing
- Beta Distribution
- Toolchains
- Rapid Development
- Deployment
- App Store
- SDK
- Xcode

####Plugins
- Package Manager
- Themes
- Misc
- Style Guides

####Good Websites
- News, Blogs and Feeds
- UIKIt references
- Components and Packages
- Forums and discuss lists
- Tutorials and Keynotes
- Prototyping
- Twitter
- Facebook Groups
- Podcasts
- Books
- Other Awesome Lists
- Contributing


#### Next up is a personal list of my favorites (essentials don't count here)
- **PromiseKit**
