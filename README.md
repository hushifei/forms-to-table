Shinobi Charts/Grids/Essentials Project Title (Objective-C/Xamarin/Android)
=====================

Description of project (include link to blog post if there is one)

![Screenshot](screenshot.png?raw=true)

Building the project
------------------

In order to build this project you'll need a copy of ShinobiCharts/Grids/Essentials. If you don't have it yet, you can download a free trial from the [ShinobiCharts/Grids/Essentials website](link to appropriate section).

Once you've downloaded and unzipped ShinobiCharts/Grids/Essentials, open up the project in XCode, and drag ShinobiCharts/Grids/Essentials.embeddedframework from the finder into Xcode's 'frameworks' group, and XCode will sort out all the header and linker paths for you.

**Delete the inappropriate sections (and alter the chart/grid name in the sample code if appropriate):**

If you're using the trial version you'll need to add your license key. To do so, open up ViewController.m and add the following line after the chart is initialised:

    chart.licenseKey=@"your license key";

If you're using the trial version you'll need to add your license key. To do so, open up ViewController.m and add the following line after the grid is initialised:

    grid.licenseKey=@"your license key";

If you’re using the trial version you’ll need to add your license key. To do so, open up AppDelegate.m, import <ShinobiEssentials/SEssentials.h>, and set the license key inside application:didFinishLaunchingWithOptions: as follows:

    #import <ShinobiEssentials/SEssentials.h>

    @implementation AppDelegate

    - (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
    {
        [SEssentials setLicenseKey:@"your license key"];
        …
    }

Contributing
------------

We use the Fork & Pull Model so if you want to contribute to this project, please go ahead and fork our repository, make your changes, then send us a pull request when you’d like us to take a look at your work.

License
-------

The [Apache License, Version 2.0](license.txt) applies to everything in this repository, and will apply to any user contributions.
