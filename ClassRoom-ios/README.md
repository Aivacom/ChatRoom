# iOS Tutorial for Objective-C - Education

中文版本：[简体中文](README.zh.md)

This open source sample project demonstrates the related functions of the demo of the interactive live broadcast large class scene.

## 1 Project Description

The interactive live big class is a Demo example based on the educational scene. You can compile and run the sample code to experience it. The following functions are included in this sample project：

- Classroom management；
- Real-time audio and video interaction；
- Send and receive real-time messages；
- Whiteboard；

## 2 Environmental preparation

- XCode 10.0 +
- iOS 8.0 +
- iPhone Device

## 3 Run the sample program

This section mainly explains how to compile and run the sample code.

### Create a developer account and get AppId

Before compiling and starting the example program, you need to first obtain an available AppId:

1. Create a developer account in [Developer Platform](https://docs.aivacom.com/cloud/cn/platform/console/registration_and_login/registration_and_login.html)
2. Go to the project management page and click the *Project management* menu in the left navigation bar to create your project. Refer to [Create and Manage Projects](https://docs.aivacom.com/cloud/cn/platform/console/create_and_manage_projects/create_and_manage_projects.html)
3. Copy the AppId of your project

   
### Configure AppId and related tokens in the project

1. Find the SYAppConfig.plist file according to the directory SCClassRoom->Demo->AppConfig
2. Fill in the AppID of your project in the `app_id` configuration in the SYAppConfig.plist file
3. Fill in `sdk_token` in SYAppConfig.plist. For the method of obtaining Token, please refer to [User Authentication](https://docs.aivacom.com/cloud/cn/platform/other/user_auth.html) and [Generate Authentication Token ](https://docs.aivacom.com/cloud/cn/product_category/rtc_service/rt_video_interaction/common_functions/generate_token/generate_token_java.html)
4. Fill in `white_url` and` white_token` in SYAppConfig.plist, please log in to [Herewhite](https://console.herewhite.com/) official website

Note：
> If you have not deployed a Token server, it is recommended that you set the project to [AppID authentication mode](https://docs.aivacom.com/cloud/cn/platform/console/create_and_manage_projects/create_and_manage_projects.html)

> If you do not need the whiteboard function, you can not fill in the `white_url` and` white_token` parameters in the SYAppConfig.plist file

### Integrate dependent SDK

1. Install CocoaPods, enter the following command line in Terminal：  
    > brew install cocoapods  
* If you have installed CocoaPods and Homebrew in your system, you can skip this step.
* If Terminal displays -bash: brew: command not found, you need to install Homebrew before entering the command line. See the Homebrew installation method for details. 

2. Use the terminal to enter the sample code project directory and execute the 'pod update' command;
3. Use Xcode to open SCClassRoom.xcworkspace, connect the iPhone / iPad device, set a valid developer signature and BundleId to run;

## Contact us

- If you want to know more official examples, you can refer to [official sample code](https://github.com/Aivacom?tab=repositories)
- For the complete API documentation, see [RTC official documentation](https://docs.aivacom.com/cloud/cn/product_category/rtc_service/rt_video_interaction/api/Android/v2.8.0/category.html) and [RTS official documentation](https://docs.aivacom.com/cloud/cn/product_category/rtm_service/instant_messaging/api/Android/v3.1.4/category.html)