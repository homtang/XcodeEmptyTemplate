Xcode 6 has removed the Empty Application template, this can help you to create Empty Application template in Xcode 6.

Copy `Empty Application.xctemplate` folder to `~/Library/Developer/Xcode/Templates/`

Now you can create empty template in Xcode 6.

Then open `AppDelegate.m` and edit `applicationDidFinishLaunchingWithOptions`

Swift:  

    func application(application: UIApplication, didFinishLaunchingWithOptions launchOptions: [NSObject: AnyObject]?) -> Bool 
    {
        self.window = UIWindow(frame: UIScreen.mainScreen().bounds)
        self.window?.backgroundColor = UIColor.whiteColor()
        self.window?.makeKeyAndVisible()
        return true
    }

Objective-C:

    - (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
    {
        self.window = [[UIWindow alloc] initWithFrame:[[UIScreen mainScreen] bounds]];
        // Override point for customization after application launch.
        self.window.backgroundColor = [UIColor whiteColor];
        [self.window makeKeyAndVisible];
        return YES;
    }