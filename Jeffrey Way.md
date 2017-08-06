# Jeffrey Way - Slay the Beast

Nine considerations to get your app back on track

## Stop asking, tell
Tell the object what you want instead of asking.

## Single use traits
User is the first candidate for abuse, what if instead we created a trait to group actions. 

No need to apologize for extracting. 

## Give it a name
- Find repeated suffixes or prefixes
- Make it a citizen in the app
- The API takes precedence always
- Maybe it could be a model or something? Refactor later

## View Polymorphism
- Pay attention to lengthy conditionals
- Use polymorphism: include($nameofview)

## Upgrade to first class
- Seek method name with same prefix, create a class with prefix as method
- Add these classes in array on main class, run a loop to trigger the method on each class

## Make it a rule
Validation rule if make sense

## Make an announcement
- Encapsulate on the class, or
- Events Event::dispatch($reply);
- Notifiable accepts a collection of users
- Only refactor towards events, sometimes it is easier to do straight in the controller/model
- PDD: Pain Driven Development
- Could use decorator passing the model as param to replace simple events

## Apply some decor
- Could use decorator instead of events, just to add behaviour to the model
- Simple delegator to make the decorator inherit the behaviour

## Query Object
- For complex queries, create a query object
- Could use __invoke to trigger function when calling the class as a function
- Can be injected in the controller


----
- Default to **Clarity**
- Don’t try to impress
- Simplest way to get the job done
- Let the grossness guide you towards a refactor
- Revert when the refactor didn’t help
- Future proof system: easy and fun to kill code
