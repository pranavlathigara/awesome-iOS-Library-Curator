# My Curated Awesome iOS Library 
A review of each project I "Star" On Github. 

As you can tell from my profile, I "STAR" more projects than prety much anyone else (I have a problem?) This document is an attempt to break down each and every one of these projects. Note that I primarily use Obj-C and this list clearly reflects that. I will make a seperate list for Swift projects

#### Note: Please also see these other awesome lists! [AwseomeUI](https://github.com/cjwirth/awesome-ios-ui), [Awesome iOS](https://github.com/vsouza/awesome-ios), [Awesome iOS Charts](https://github.com/sxyx2008/awesome-ios-chart), [Awesome iOS Animation](https://github.com/sxyx2008/awesome-ios-animation), [Awesome iOS Top 1000](https://github.com/iamdaiyuan/ios_top_1000) , [Awesome_WatchOS](https://github.com/sanketfirodiya/sample-watchkit-apps), [Awesome Swift](https://github.com/matteocrippa/awesome-swift), and this other [Awesome Swift](https://github.com/Wolg/awesome-swift) . A huge thanks is also in order for Cocoapods and CocoaControls - I wouldn't be the dev I am today without learning from a few projects I picked up from each of those sites.
#### Please also know this was not meant to discredit any other lists!! This list is just my own expanded version of those, so that I can put my own 2 cents on each library. It was created to help me remember what I have seen on Github - there is an incredible open source community out there that could really save you tons of time if you use it right! Hopefully this list can be a bit helpful for you

This guide was created using **[Prose](http://prose.io/)**, which utilizes [**Markdown**](https://confluence.atlassian.com/display/STASH/Markdown+syntax+guide?continue=https%3A%2F%2Fconfluence.atlassian.com%2Fdisplay%2FSTASH%2FMarkdown%2Bsyntax%2Bguide&application=cac) style syntax. 

## **Index**

Here's how this list is going to be categorized:
- Essential Projects
- ReactiveCocoa / FRP / MVVM intro
- ReactiveCocoa Projects
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
- **[Typhoon](https://github.com/appsquickly/Typhoon)**: Another D.I. framework that people really really love
- **[Specta](https://github.com/specta/specta)**: A light-weight TDD / BDD framework for Objective-C & Cocoa. This makes testing your code a piece of cake
- **[Expecta](https://github.com/specta/expecta/)**: A matcher framework that works fantastically with Specta. expect(**expecta**).to.beAwesome() for testing your ReactiveCocoa code
- **[OCMock](http://ocmock.org/)**: Library for easy creation of mock objects
- **[KIF](https://github.com/kif-framework/KIF)**: Keep it functional with KIF. A great great lib for UI testing and continuous integration testing 
- **[PonyDebugger](https://github.com/square/PonyDebugger)**: Note- I added this because it looks awesome. But still testing and need to verify its awesomeness. Pretty much lets you monitor network activity with Chrome Developer Tools
- **[CocoaLumberjack](https://github.com/CocoaLumberjack/CocoaLumberjack)**: Note: see PonyDebugger. But looks easy to use and awesome. I've been using Aspects up to this point but will start looking in this direction! According to the docs, "In most cases it is an order of magnitude faster than NSLog."
- **[FLEX](https://github.com/Flipboard/FLEX)**: See PonyDebugger. FLEX looks like an ultra awesome UI debugging tool built by Flipboard. Possibly outdated? Will investigate
- **[CocoaAsyncSocket](https://github.com/robbiehanson/CocoaAsyncSocket)**: Webscokets done right in iOS
- **[CanvasPod](https://github.com/CanvasPod/Canvas)**: Really cool addition to Xcode lets you animate your stuff in interface builder WITHOUT running your code! Saves a heck of a lot of time

### Here is a list of my favorite iOS blogs and websites
- NSHipster
- Objc.io
- raywenderlich.com
- Yalantis (probably the best iOS contractors out there)
- Atomic object (I find myself on that site pretty often)
 
### Here is a list of some high quality iOS reads on how to make some high quality stuff
- [pull to make soup](https://yalantis.com/blog/how-we-built-customizable-pull-to-refresh-pull-to-cook-soup-animation/?utm_source=github)


### ReactiveCocoa, Functional Reactive Programming, and MVVM isn't easy to understand (especially for an Object Oriented developer), so here's a few good things to read first (I've read a lot of these)
- **[Zweitag FRP Breakdown](https://www.zweitag.de/en/blog/technology/functional-reactive-programming-frp)**: Before you jump into RAC, it's probably a good idea to learn a thing or 2 about what functional programming really is
- **[RXMarbles](https://github.com/staltz/rxmarbles)**: Really cool demonstrations of reactive programming operators in RX
- **[Atomic Object](http://spin.atomicobject.com/?s=reactivecocoa)** Bunch of articles from a really respected iOS development consultant group
- **[Yalantis Reactive Programming Objective-C](https://yalantis.com/blog/reactive-programming-on-objective-c/)**: Some great examples and visuals are abundant 
- [**How I Learned to Write Custom Signals in Reactive Cocoa**](https://yalantis.com/blog/how-i-learned-to-write-custom-signals-in-reactive-cocoa/): RACSignal Tutorial
- **[ifNotApps](http://ifnotapps.com/2013/08/10/reactivecocoa-from-the-ground-floor-part2/)**: Great overall breakdown. Comes with this practice project which has tons of various exmaples **_[RACExample](https://github.com/tLewisII/RACExample)_**
- **[ExpressiveReactiveCocoa](https://github.com/kastiglione/ExpressiveReactiveCocoa)**: Before you do anything RAC related, make sure to give this presentation a peak!
- **[RACDesignPatterns](http://rcdp.io)**: Definitely not the best site in the world, but I thought it was worth a read through. Definitely a conecpt that needs to be expanded on
- **[RAC Performance](https://github.com/ReactiveCocoa/ReactiveCocoa/issues/1503)**: Investigation of RAC performance
- **[RAC + MVVM introduction](http://www.sprynthesis.com/2014/12/06/reactivecocoa-mvvm-introduction/)**: One of the clearest write-ups I've ever seen. Great visuals 
- **[Modern Concurrency: Erlang, Scala, Go, Clojure](http://kachayev.github.io/talks/kharkivpy%230/#/)**: Really good presentation about what makes functional programming awesome in other languages. Let me just try to summarize quickly with some talking points
- - Remember, concurrency is not parallelism! 
- - Also, locks are awful. 
- - "Actor" is a state (Scala) VS. passing state as an argument (Erlang).
- - > "Rough analogy: writing to a file by name (process, Erlang) vs. writing to a file descriptor (channel, Go)." (c) Rob Pike 
- - Why functional programming matters in Clojure: Side-effect free functions and Deterministic functions/calculations
- - There is no silver bullet
 -- Use most natural approach for your technology / OP (there are many STM implementations, but in Clojure it's idiomatic and part of the core)
-- Look deeply into your domain (presenters usually use most convenient case(s) to tell about functionality)
-- Use "unusual" approach but remember that on this way only conventions rule
If you need distributed concurrency - look at actors
- - For Scala developers from 
Jonas Boner
:
Start with deterministic, declarative, immutable core
-- Add indeterminism selectively (actors)
-- Add mutability selectively (STM)
-- Finally: add locks and explicit threads
-- check out these [slides](https://github.com/kachayev/talks/tree/master/kharkivpy%230)
- **[twocentstudios](http://twocentstudios.com/blog/2014/06/08/on-mvvm-and-architecture-questions/)**: a friendly, project based introduction to RAC
- **[RAC TableView Binding](http://blog.scottlogic.com/2014/05/11/reactivecocoa-tableview-binding.html)**: An exploration of using RAC to update the contents of a UITableView
- **[Ray Wenderlich](http://www.raywenderlich.com/62699/reactivecocoa-tutorial-pt1)**: Some people like these
- **[Ash Furrow Video](https://www.youtube.com/watch?v=TlgUWYrQ0sc)**: Great presentation by one of RAC's leading voices
- **[Cocoa Samuri](http://cocoasamurai.blogspot.ca/2013/03/basic-mvvm-with-reactivecocoa.html)**: Introduction that everyone is referring to
- **[Reactive Cookbook](http://reactivecookbook.com/)**: Cookbook for a few reactive cococa things. Comes with this [example](https://github.com/jeroenvloothuis/Reactive-Cookbook)
- **[Bi-directional data bindings with RACChannel](http://spin.atomicobject.com/2015/05/04/bi-directional-data-bindings-reactivecocoa/)**: If you want to really push your knowledge of RAC, this is an interesting read
- [**RAC Changelog**](https://github.com/ReactiveCocoa/ReactiveCocoa/blob/fd533d07b64d40cf79d069584d8cd95158998095/CHANGELOG.md#simpler-two-way-bindings): You've probably already read the RAC documentation (highly recommended). However, you probably haven't read [this](https://github.com/ReactiveCocoa/ReactiveCocoa/blob/fd533d07b64d40cf79d069584d8cd95158998095/CHANGELOG.md#simpler-two-way-bindings)
- [**Reactive Cocoa and Ruby Motion**](http://spin.atomicobject.com/2013/06/18/reactivecocoa-rubymotion/): If you HAVE to use Ruby Motion, you might want to check out this set up guide for getting your RAC code up and running

### ReactiveCocoa should transform EVERYTHING when it comes to writing iOS code so here's a bunch of projects that should make your RAC transtion a little bit smoother

- **[Functional Reactive Pixels (FRP)](https://github.com/ashfurrow/FunctionalReactivePixels)**: A great project from the zen master Ash Furrow. Featured in his book
- **[ExpressiveReactiveCocoa](https://github.com/kastiglione/ExpressiveReactiveCocoa)**: Before you do anything RAC related, make sure to give this presentation a peak!
- **[RACAction](https://github.com/Automatic/RACAction)**: Make your RACCommands look like Swith and RAC 3.0 's RACAction!
- **[101 RAC Samples](https://github.com/dogwith1eye/101RACSamples)**: 101 different examples of using RAC :)
- **[Bizhi](https://github.com/lzyy/bizhi)**: the holy grail of example projects. uses objection + reactivecocoa (my favs) + AFNetworking + UICollectionView
- **[Typhoon + Core Data + RAC](https://github.com/appsquickly/Typhoon-CoreData-RAC-Example)**: The holy grail for those who prefer Typhoon over aObjection
- **[RateStuff](https://github.com/danbennett/RateStuff)**: Another RAC + Typhoon example
- **[Firebase + RACExtensions](https://github.com/joenoon/Firebase-RACExtensions)**: a lib that adds extension abilities to Firebase. I find this ultra awesome for dynamic user interfaces in need of live updates
- **[UIGestureRecognizer-RACExtension](https://github.com/kaiinui/UIGestureRecognizer-RACExtension)**: Adds UIGestureRecognizer extensions to RAC
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
- **[*RACCommandExample](https://github.com/olegam/RACCommandExample)**: An incredibly insightful example project that accompanies this blog [post](http://codeblog.shape.dk/blog/2013/12/05/reactivecocoa-essentials-understanding-and-using-raccommand/) 
- **[AFNetworking-RACExtensions](https://github.com/CodaFi/AFNetworking-RACExtensions)**: Incredibly helpful RACifying AFNetworking code! Would be pretty difficult to build by yourself (check out this blog [post](http://codeblog.shape.dk/blog/2013/11/16/wrapping-afnetworking-with-reactivecocoa/) too)

		AFHTTPRequestOperationManager *manager = [[AFHTTPRequestOperationManager alloc] initWithBaseURL:url];
		manager.requestSerializer = [AFJSONRequestSerializer serializer];
		manager.responseSerializer = [AFJSONResponseSerializer serializer];
		[[manager rac_GET:path parameters:params] subscribeNext:^(RACTuple *JSONAndHeaders) {
    			//Voila, a tuple with (JSON, HTTPResponse)
		}];
		
- **[SKPKeyboardAwareness](https://github.com/shapehq/SHPKeyboardAwareness)**: Aha! Now we really can see some power of RAC. This lib uses it to understand the presence of a keyboard (which is really annoying ususally)
		// shpka_rac_notifyUntilDealloc is our own convenience method that returns
		// a signal with a notification that completes when the receiver deallocates.
		RACSignal *keyboardSignal = [self shpka_rac_notifyUntilDealloc:UIKeyboardWillShowNotification];

		// viewSignal is a signal that fires whenever a UITextField or UITextView becomes first responder.
		RACSignal *viewSignal = [RACSignal merge:@[
  		[self shpka_rac_notifyUntilDealloc:UITextFieldTextDidBeginEditingNotification],
		  [self shpka_rac_notifyUntilDealloc:UITextViewTextDidBeginEditingNotification]]
		];
		// The two signals above, combined in a ‘zip’, meaning that one of the zipped signals
		// will wait for the other before combinedShowSignal is fired.
		RACSignal *combinedShowSignal = [RACSignal zip:@[viewSignal,keyboardSignal]];

- **[MVVM iOS Example](https://github.com/Machx/MVVM-IOS-Example)**: Solid introduction to the MVVM design pattern
- **[ReactiveCocoa-IO](https://github.com/ReactiveCocoa/ReactiveCocoaIO)**: Use RAC for file IO!!
- **[RAC-Parse](https://github.com/kastiglione/Parse-RACExtensions)**: If you're dumb enough to use Parse, then you better use RAC - you're gonna need it!
- **[RAC-Example](https://github.com/tLewisII/RACExample)**: Another example. Nt bad
- **[RAC-Playground](https://github.com/Machx/Reactive-Cocoa-Playground)**: Someone's playground project
- **[Expecta+RAC](https://github.com/kylef/Expecta-ReactiveCocoa)**: LOVE THIS. Expecta is the testing framework that's great for MVVM. It only makes sense to add RAC support!
- **[LLRreactiveMatchers](https://github.com/lawrencelomax/LLReactiveMatchers)**: Just like the one above. LLReactiveMatchers should be able to cover most of the reasons you want to test Signals. One matcher = One Subscription, n Matchers = n Subscriptions. Tests that compose on top of Subjects should use LLSignalTestRecorder and expectations should be made on the recorder.

    		NSMutableArray *sentValues = [NSMutableArray array];
    		NSArray *expected = @[@0, @1, @2];
    		BOOL hasCompleted = NO;
    	        [signal subscribeNext:^(id value) {
		    [sentValues addObject:value];
    		} completed:^{
		    hasCompleted = YES;
    		}];
    		expect(hasCompleted && [sentValues isEqualToArray:expected]).will.beTruthy();
    		
- **[RAC+BLE](https://github.com/indragiek/ReactiveBLE)**: RAC support for Buletooth low energy communication with core bluetooth
- **[Simple Weather](https://github.com/TCLee/ReactiveWeather)**: Awesome test project that uses RAC and Mantle
- **[RAC+RestKit](https://github.com/stefanomondino/SMReactiveRestKit)**: RAC support for RestKit- awesomeness. RestKit is a framework for consuming and modeling RESTful web resources on iOS and OS X
- **[Ash Furrow Func Reactive Demo](https://github.com/ashfurrow/FunctionalReactiveDemo)**: Because ash furrow. A small demonstration of how to use ReactiveCocoa in iOS applications
- **[RAC+Healthkit](https://github.com/kerryknight/ReactiveHealthKit)**: Because it's awesome to get live health updates
- **[RAC+Pull-To-Refresh](https://github.com/iandundas/SimpleReactiveTableViewExample)**: Demonstrates networking, JSON parsing, displaying in a tableView and implementing pull-to-refresh using ReactiveCocoa, also laid out using MVVM pattern
- **[RAC+Accounts Framework](https://github.com/ikesyo/ReactiveAccountStore)**: RACSupport for Accounts
- **[RAC+AlertAction](https://github.com/ashfurrow/RACAlertAction)**: Ash Furrow made it. Pretty useful for this scenario
- **[RAC+Notification](https://github.com/mpurbo/MMPReactiveNotification)**: RAC for push notis
- **[RAC+Reachability](https://github.com/kaiinui/Reachability-RACExtensions)**: Needs work but you get the idea
- **[Loverly](https://github.com/moyunmo/Loverly)**: AFNetworking, ReactiveCocoa+MVVM, Pop
- **[RAC+Evernote](https://github.com/rizumita/Reactive-Evernote-SDK-iOS)**: For the Evernote SDK
- **[RACSnippets](https://github.com/lzyy/RAC-Snippets)**: Various RAC Snippets. This project is really really good. Possibly my favorite RACExample project. It has a whole bunch of different cases in which you might use RAC. These cases are listed below
	- Use 'then' and 'take' 
    - Simple MVVM
    - Notification with RAC
    - UITableView and reloadData
    - Waterfall (with SDWebImage)
    - RAC and RACObserve and map
    - use 'tryMap'
    - Repeat after TimeInterval
    - RACCommand
    - Auto Fetch access token
    - Use TakeUntil with Cell
    - Deal Multiple Errors

- **[RAC+PullToRefresh](https://github.com/WilliamZang/ZCWRACPullRefresh)**: Refresh control written in RAC
- **[C-41](https://github.com/ashfurrow/C-41)**: Yet another fantastic Ash Furrow project. This guy seriously knows his stuff. This project is great not only in it's completeness, but also because it is fully tested with Expecta, Specta, and OCMock
- **[Reactive Cocoa Playground](https://github.com/Machx/Reactive-Cocoa-Playground)**: Made by the guy who made that highly quoted MVVM article. Lots of really good examples

##### Wow - you might be saying to yourself... "THERE'S SO MANY PROJECTS!" OKAAY. I'LL LIST MY FAVORITE ONES IN ORDER

##### RAC Example Projects
1. RACSnippets
2. Functional Reactive Pixels (Ash Furrow)
3. C-41 (Ash Furrow)
4. RACExample 
5. 101 RAC Examples
6. Artsy/Eigen (Ash Furrow)
7. Func Reactive Demo (Ash Furrow)
8. RACCommand Example
9. Bizhi
10. Reactive Cocoa Playground 
11. Bikes
 

##### RAC+Extensions
1. AFNetworking + RACExtensions
2. Expecta + RAC
3. CETableViewBinding

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
- **JazzHands**

#### Thanks for checking out this post! Here are some more awesome pages
- [**awesome-xamarin**](https://github.com/benoitjadinon/awesome-xamarin)
- awesome-AndroidUI
- **[Awesome_AngularJS](https://github.com/gianarb/awesome-angularjs)**
- just an awesome AngularJS [website](https://angularjs.zeef.com/gianluca.arbezzano)
- **Awesome [Javascript](https://github.com/sorrycc/awesome-javascript)**
