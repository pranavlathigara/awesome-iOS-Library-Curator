# My Curated Awesome iOS Library 
A review of each project I "Star" On Github. 

As you can tell from my profile, I "STAR" more projects than prety much anyone else (I have a problem?) This document is an attempt to break down each and every one of these projects. Note that I primarily use Obj-C and this list clearly reflects that. I will make a seperate list for Swift projects

#### Note: Please also see these other awesome lists! [AwseomeUI](https://github.com/cjwirth/awesome-ios-ui), [Awesome iOS](https://github.com/vsouza/awesome-ios), [Awesome iOS Charts](https://github.com/sxyx2008/awesome-ios-chart), [Awesome iOS Animation](https://github.com/sxyx2008/awesome-ios-animation), [Awesome iOS Top 1000](https://github.com/iamdaiyuan/ios_top_1000) , [Awesome_WatchOS](https://github.com/sanketfirodiya/sample-watchkit-apps), [Awesome Swift](https://github.com/matteocrippa/awesome-swift), and this other [Awesome Swift](https://github.com/Wolg/awesome-swift) . A huge thanks is also in order for Cocoapods and CocoaControls - I wouldn't be the dev I am today without learning from a few projects I picked up from each of those sites.
#### Please also know this was not meant to discredit any other lists!! This list is just my own expanded version of those, so that I can put my own 2 cents on each library. It was created to help me remember what I have seen on Github - there is an incredible open source community out there that could really save you tons of time if you use it right! Hopefully this list can be a bit helpful for you

This guide was created using **[Prose](https://github.com/prose/prose)**, which utilizes [**Markdown**](https://confluence.atlassian.com/display/STASH/Markdown+syntax+guide?continue=https%3A%2F%2Fconfluence.atlassian.com%2Fdisplay%2FSTASH%2FMarkdown%2Bsyntax%2Bguide&application=cac) style syntax. 

## **Index**

Here's how this list is going to be categorized:
- Essential Projects
- ReactiveCocoa Extensions
- Library and Frameworks
- Plugins
- Good Websites
- My Personal Favorites
- Example Projects (to be broken down furthur)
- Awesome iOS Reads

### First, the gold standard libraries. The essentials --- You **NEED** to know about these !! You're likely to include a few of these in your own iOS projects

- **[AFNetworking](https://github.com/AFNetworking/AFNetworking)**: Probably the most "starred" iOS project on Github, and for good reason. AFNetworking wraps most of the complicated NSURLSession / HTTP / Core Data into one easy to use library.
- **[ReactiveCocoa](https://github.com/ReactiveCocoa/ReactiveCocoa)**: If you haven't heard about this one, well, you're in for a serious treat. This lib makes your iOS code _Functional_ and _Reactive_. Find out more from their documentation on their github page or from their [website](http://reactivecocoa.io/)
- **[Mantle](https://github.com/Mantle/Mantle)**: A fantastic lib for creating Model objects in iOS. Normally, this requires a ton of boilerplate code. Now, it doesn't have to!
- **[GPUImage](https://github.com/BradLarson/GPUImage)**: The single best lib when it comes to editing images. 
- **[POP](https://github.com/facebook/pop)** Easily the best UI Lib ever built for iOS. Built by Facebook - it provides and alternative to working with the super obnoxious CoreAnimation and UIKitDynamics libs. Do cool spingy stuff!
- **[RESTKit](https://github.com/RestKit/RestKit)**: A fantastic library for making REST type requests in iOS with WEB services relatively painless. It provides a powerful object mapping engine that seamlessly integrates with Core Data and a simple set of networking primitives for mapping HTTP requests and responses built on top of AFNetworking. It has an elegant, carefully designed set of APIs that make accessing and modeling RESTful resources feel almost magical.
- **[MagicalRecord](https://github.com/magicalpanda/MagicalRecord)**: Inspired by Martin Fowler's ActiveRecord pattern, where data is stored in relational databases, Magical Record is a lib that simplifies all of your Core Data code. With MagicalRecord, database and object communication is made a heck of a lot easier. Which is great, because I personally get headaches wrapping my head around Core Data. Reminds me of R.O.R.'s ActiveRecord response to CRUD, using an NSFetchedResultsController
- **[Masonry](https://github.com/SnapKit/Masonry)**: You got autolayout issues? Don't like using storyboards? Hate autolyout code? (I know I do!) Use this library instead! 
- **[Objection](http://objection-framework.org/)**: Dependency Injection in objective-c made so much easier with this. A great great lib that fixes one of my least favorite parts of the ojective-c language.
- **[Specta](https://github.com/specta/specta)**: A light-weight TDD / BDD framework for Objective-C & Cocoa. This makes testing your code a piece of cake
- **[Expecta](https://github.com/specta/expecta/)**: A matcher framework that works fantastically with Specta. expect(**expecta**).to.beAwesome() for testing your ReactiveCocoa code
- **[OCMock](http://ocmock.org/)**: Library for easy creation of mock objects
- **[KIF](https://github.com/kif-framework/KIF)**: Keep it functional with KIF. A great great lib for UI testing and continuous integration testing 
- **[PonyDebugger](https://github.com/square/PonyDebugger)**: Note- I added this because it looks awesome. But still testing and need to verify its awesomeness. Pretty much lets you monitor network activity with Chrome Developer Tools
- **[CocoaLumberjack](https://github.com/CocoaLumberjack/CocoaLumberjack)**: Note: see PonyDebugger. But looks easy to use and awesome. I've been using Aspects up to this point but will start looking in this direction! According to the docs, "In most cases it is an order of magnitude faster than NSLog."
- **[FLEX](https://github.com/Flipboard/FLEX)**: See PonyDebugger. FLEX looks like an ultra awesome UI debugging tool built by Flipboard. Possibly outdated? Will investigate
- **[CocoaAsyncSocket](https://github.com/robbiehanson/CocoaAsyncSocket)**: Webscokets done right in iOS

### Next, because ReactiveCocoa should transform EVERYTHING when it comes to writing iOS code, here's a few extensions that should make your RAC transtion a little bit smoother

- **[Firebase + RACExtensions](https://github.com/joenoon/Firebase-RACExtensions)**: a lib that adds extension abilities to Firebase. I find this ultra awesome for dynamic user interfaces in need of live updates
- **[ReactiveCocoaLayout](https://github.com/ReactiveCocoa/ReactiveCocoaLayout)**: an awesome lib for creating animations with ReactiveCocoa
- **[ReactiveViewModel](https://github.com/ReactiveCocoa/ReactiveViewModel)**: a library that shows, by example, how to use the MVVM design pattern
- **[ReactiveCoreData](https://github.com/apparentsoft/ReactiveCoreData)**: Below is an example of how this lib can be used. ReactiveCocoaLayout brings RAC code to the most obnoxious parts of iOS ibrary (I'm looking at you, autolayout!)

            RAC(self.filteredParents) = [[[[Parent findAll]
              where:@"name" contains:filterText options:@"cd"]
              sortBy:@"name"]
              fetchWithTrigger:objectsChanged];

- **[CETableViewBinding](https://github.com/ColinEberhardt/CETableViewBinding)**: A library that makes the somewhat overwhleming task of using RAC with UITableViews less obnoxious
- **[Bikes](https://github.com/edc1591/Bikes)**: A great example project for proper use of the MVVM pattern built by some guy over at TimeHop
- **[Reactive+iBeacon](https://github.com/eliperkins/ReactiveBeacon)**: Very Very cool lib that makes your iPhone discoverable in an NFC environment
- **[MMPReactiveCoreLocation](MMPReactiveCoreLocation)**: CoreLocation annoyances made less annoying with RAC
- **[LibExtobj](https://github.com/jspahrsummers/libextobjc)**: This is a library that gives you some cool little additions, most notably @weakify(self) and @strongify(self)
- **[OctoKit](https://github.com/octokit/octokit.objc)**: A massive project undertaking from the makers of RAC. A good project to look at if you need ideas on RAC
- **[Artsy/Eigen](https://github.com/artsy/eigen)**: From one of RAC's biggest supporters, Ash Furrow

### Recently I've done a few projects that involve Payments, iBeacons, and PassKit. Make sure to check these links out:
- **[Ubudu](https://github.com/Ubudu/IOS-SDK)**: Cool SDK for integrating iBeacons into your retail space. Looks good for malls ($$$)
- **[Captainpass](https://github.com/CarvingLabs/captainpass-ios-sdk)** Simple to use Passbook sdk ($$$)
- **[PassSlot](https://github.com/passslot/passslot-ios-sdk)**: Another passbook SDK ($$$)
- **[PassKit](https://passkit.com/)**: This one looks like the real deal. They use iBeacons, rewards and everything. However, might be overkill. How did they score that name ??
- **[LevelUp](https://github.com/Level/levelup)**: One of the best systems I've seen. Costs money, however


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

#### Plugins
##### Package Manager
- **[xctool](https://github.com/facebook/xctool)**: Tool to run xcode builds much more easily through the terminal.

##### Themes
##### Misc - Below are some tools that I'd recommend for you to really familiarize yourself with

-**[SYNX](https://github.com/venmo/synx)**: This cleans up your project folder... automatically! One of those wicked cool Ruby scripts that makes sure your Xcode project folder matches what you have in your Xcode project. Any unused junk files get automatically deleted!


##### Style Guides

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
- Other Awesome Lists
- Contributing

#### Awesome iOS Books (because, sometimes I read?)

#### Next up is a personal list of my favorite libraries (essentials don't count here)
- **PromiseKit**

#### Last up is a personal list of my favorite projects (essentials don't count here)
- **[CBStoreHouseRefreshControl](https://github.com/coolbeet/CBStoreHouseRefreshControl)**: This may be one of the coolest refresh controls I've ever seen
- **[JVFloatLabeledTextField](https://github.com/jverdi/JVFloatLabeledTextField)**: Easily the coolest text field I've ever seen
- **[SlackTextViewController](https://github.com/slackhq/SlackTextViewController)**: The best message view controller I've ever seen
-


#### Thanks for checking out this post! Here are some more awesome pages
- [**awesome-xamarin**](https://github.com/benoitjadinon/awesome-xamarin)
- awesome-AndroidUI
- **[Awesome_AngularJS](https://github.com/gianarb/awesome-angularjs)**
- just an awesome AngularJS [website](https://angularjs.zeef.com/gianluca.arbezzano)
- **Awesome [Javascript](https://github.com/sorrycc/awesome-javascript)**
