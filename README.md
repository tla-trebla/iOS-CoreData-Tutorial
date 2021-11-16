# iOS-CoreData-Tutorial
Learn how to use Core Data in Swift based on article "Getting Started with Core Data Tutorial" by Ray Wenderlich.
Link: https://www.raywenderlich.com/7569-getting-started-with-core-data-tutorial#toc-anchor-004

# Things I've Learned
* There's a Data Model Editor to create a new Entity & a new Attributes inside the Entity.
* Entity is a class definition on Core Data.
* Attributes is a piece of information inside the Entity.
* Relationship is a communication between Entities (one-one, many-many, & one-many relationship).
* To fetch or save data at Core Data, we should call the managed object context.
* Saving to Core Data should call a Managed Object with Entity (NSEntityDescription) and managed context.
  * When creating the NSEntityDescription, by default it's an optional variable, and should be force unwrapped.
  * When set a value on the Entity's property, it should be exactly the same name. Unless the app will be crashed.
* Fetching from Core Data should call a Fetch Request that returns a managed object (NSManagedObject) with Entity's name.
* Best practice fetching at the overridden method named "viewWillAppear".
* When fetching or saving at Core Data with a managedContext, implement it with a do-catch implementation.
