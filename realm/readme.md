# Realm

### Realm Instance Lifecycle
Choosing the proper lifecycle for a Realm instance is a balancing act. Because RealmObjects and RealmResults are accessed through a lazy cache, keeping a Realm instance open for as long as possible not only avoids the overhead incurred in opening and closing it but is likely to allow queries against it to run more quickly. On the other hand, an open Realm instance holds significant resources, some of which are not controlled by the Java memory manager. Java cannot automatically administer these resources. It is essential that code that opens a Realm instance closes it when it is no longer needed.


### Best Practice to use Realm instance


### React Component lifecycle & Navigation lifecycle events
while React's lifecycle methods are still valid, React Navigation adds more lifecycle events that you can subscribe to through the navigation prop.
you may also use the withNavigationFocus HOC or <NavigationEvents /> component to react to lifecycle changes

### AppState - Native React lifecycle
background/inactive/..
