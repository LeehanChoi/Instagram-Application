# Instagram-Application
### Leehan's Instagram Application 

#### 1. Create new project.
* In this process, you need to **be careful** with the choice of Interface **'Storyboard'**.
if you are not selected, then 'AppDelegate', 'SceneDelegate', 'ViewController' will not be created.

#### 2. Create some folders to start organizing project.
* Create New groups below 
* Controllers / Views / Models(data layer) / Resources (hold everything that doesn't fit into these other three folders) 

**As your projects get larger especially with big projects if you don't organize early on you end up in quite a bind.**

#### 3. Organization
* move 'AppDelegate', 'SceneDelegate' to Resources folder.
* move 'ViewController' to Controllers folder. 
* move 'Main', 'Assets', 'LaunchScreen' to Views folder.
* create new group 'Storyboards' below the Views folder, including 'Main', 'LaunchScreen'.

* Go Views -> Storyboards -> Main -> View Controller Scene -> View Controller -> attribute inspector -> Custom class -> change the name 'HomeViewController' as well. 
* b/c this template was set up with that original controller we want to change the name here in the storyboard.

#### 4. Rename this controller that was given to us.
* It's called 'ViewController' very vague and generic. So we're going to update all of these names.
* Go Controllers -> ViewController -> renamed 'HomeViewController'

#### 5. Create four more controllers
* Controllers folder 
* click new file cocoa touch class -> named 'ExploreViewController' / 'CameraViewController' / NotificationViewController' / 'ProfileViewController' / 
* let's delete commented out code as we go along since we don't need it. 
* These five controllers will basically serve as our core app experience. 
* select five controllers and create a new group name 'Core Tabs' (below Controllers folder).

#### 6. Create New folder below Controllers folder.
* new group named 'Other' 
* create new group 'Onboarding' below 'Other'.
* 'Onboarding' is going to basically be either the login screen or the registration screen.
* create new files below Onboarding folder - 'LoginViewController', 'RegistrationViewController'

* when you tap on a post it actually opens up another screen which is more details about one focused post. so we're gonna do a new file below Other folder - 'PostViewController', this is going to be the screen where if you tap into a post, it actually just shows the information about that post. / 'EditProfileViewController' / 'SettingsViewController' / 'ListViewController' / 'SearchViewController' / 'SearchResultViewController' / 'PostEditorViewController' / 'PublishPostViewController' / 


#### 7. Go to main storyboard
* get rid of this controller actually. (default iphone display)
* click + button right above the xcode. 
* create tab bar controller and then delete two controllers that are connected to it.
* create navigation controller and then delete Table View that is connected to it. 
* select this navigation controller copy and paste it until you have five of them. 
* press control key and click and drag from Tab Bar Controller to the navigation Controller one by one. select Relationship Segue is View controller.  

* create View Controller and copy and paste it until you have five of them. 
* press control key and click and drag from Navigation Controller to the View Controller one by one. select Relationship Segue is root view controller. 

* assign a class for each of these View Controller. select that first one and come over arribute inspector and custom class 'HomeViewController'.
* next one is ExploreViewController.
* third one is CameraViewControlelr.
* fourth one is NotificationViewController.
* last one is ProfileViewController.

* select first navigation controller's item -> attribute inspector -> Tab bar item -> Bar item -> remove Title -> search Image 'House' 
* the next one is globe / plus / bell / person.
* if you want to change icons color then select item of Tab Bar Controller ->  attribute inspector -> Tab bar -> image Tint -> change color


**if xcode alerts one issue about 'Unsupported Configuration. Tab Bar Controller is unreachable because it has no entry points,....' then attribute inspector -> simulated Metrics -> View Controller -> check 'Is Initial View Controller' 

**if you want to change simulator is in dark mode <-> light mode, press command + shift + A **


#### 8. Terminal setting

