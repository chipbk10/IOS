## Topics

## System Design

### Exercise:
- [Design File Downloader Library](https://github.com/weeeBox/mobile-system-design/blob/master/exercises/file-downloader-library.md): to redo
- [Design Caching Library](https://github.com/weeeBox/mobile-system-design/blob/master/exercises/caching-library.md): to redo
- [Design Image Library](https://github.com/weeeBox/mobile-system-design/blob/master/exercises/image-library.md): to redo
- [Design Chat app](https://github.com/weeeBox/mobile-system-design/blob/master/exercises/chat-app.md): to redo
- [Design Twitter Feed](https://github.com/weeeBox/mobile-system-design): to redo

### Mock
- [Discord group](https://discord.com/invite/AWDNrvqban) for finding partners
- [List of recorded mocks](https://codeshare.io/mobiledesignmocks)

### Resource:
- [Building mobile app at scale](https://drive.google.com/drive/u/0/folders/1DuozSvEJN7-W0tY26dkhJxm1VutSO8Kn): to read (very important)

### How to support offline?
- Trello
  - [Airplane Mode](https://tech.trello.com/sync-architecture/)
  - [Sync](https://tech.trello.com/syncing-changes/)
  - [Sync Failure Handling](https://tech.trello.com/sync-failure-handling/)
  - [Sync two id problem](https://tech.trello.com/sync-two-id-problem/)
  - [Offline attachments](https://tech.trello.com/sync-offline-attachments/)
  - [Sync is a two-way street](https://tech.trello.com/sync-downloads/)
  - [Display Sync State](https://tech.trello.com/sync-indicators/)

- Azure
  - [Data Caching and Synchronization](https://www.youtube.com/watch?v=X6VdfcrDU-I&ab_channel=XamarinUniversity): to watch
  
### Handle Synchronization conflicts
- [Azure: Handle Synchronization conflicts](https://www.youtube.com/watch?v=aIuxJHq0NYY&ab_channel=XamarinUniversity): to watch
- [Google Doc](https://www.youtube.com/watch?v=B5NULPSiOGw&ab_channel=InfoQ): automerge, pullrequest

### Polling
- Polling in spotty connection, or app runs into background

### Functional Programming


### Git

## Design Pattern
- [Design Notification Center](https://github.com/100mango/SwiftNotificationCenter)

## Data Structrure and Algorithms

- [DFS](https://leetcode.com/list?selectedList=e75upz5g)
- [BFS](https://leetcode.com/list?selectedList=et5pil9r)
- [In-Order-BST](https://leetcode.com/list?selectedList=euqf8w3g)
- [BT](https://leetcode.com/list?selectedList=oncud9uc)
- [Intervals](https://leetcode.com/list?selectedList=9fsxo1iv)
- [Backtracking](https://leetcode.com/list?selectedList=ow32n1i1)
- [Two-Pointers](https://leetcode.com/list?selectedList=odn1wlys)

## iOS

### Security
- [Exploiting Common iOS Apps’ Vulnerabilities](https://www.youtube.com/watch?v=RLzbHHoEKo8&ab_channel=InfoQ): to watch

### Persistence
- Cache
  - [NSURLCache](https://nshipster.com/nsurlcache/)

### Swift
- [Quizz](https://jasper-foe-e81.notion.site/F-L-A-S-H-C-A-R-D-S-592bc284ccce4b3991aa8044705bf573): to review
- [autoclosure](https://www.swiftbysundell.com/articles/using-autoclosure-when-designing-swift-apis/)
- [frozen enum](https://useyourloaf.com/blog/swift-5-frozen-enums/)
- `static func` vs `class func`: static and class both associate a method with a class, rather than an instance of a class. The difference is that subclasses can override class methods; they cannot override static methods.

### Test
- How to call a set up method only once before running all tests? use `override class func setUp()`

### SwiftUI
- [Navigation](https://github.com/pointfreeco/swiftui-navigation)

## CI/CD

### Pipeline
- [How does XCode generate a DerivedData hash?](https://github.com/chipbk10/IOSSwiftBestPractice/blob/main/IOSSwiftBestPractice/CICD/GenerateDerivedDataHash.swift)
- SwiftLint? What is the advantage of create a separate target for SwiftLint? for standardization, and also because you don't want to run swiftlint everytime you build your target (you only need to run it at some point, as a check, but not everytime, especially on the CI, that's too expensive)
- What is the aggregate target used for?
- Sonarqube?
- Keychain doesn't allow to use different accounts to access the same base url (like www.example.com, www.example.com/home, www.example.com/category, etc.) How do we overcome it? The answer is use a custom credential provider (in keychain). It's a bit more subtle than that, like, you can configure keychain to hold different credentials for full repo url-s, but we need an intermediate thing (like dev.azure.com/<organization>). The default macos keychain handler allows only base url (dev.azure.com), or full repo-url (dev.azure.com/../../../<reponame>), but no intermediate ...and it has other disadvantages too


