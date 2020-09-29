# The-Freedom-Wrapper-Project

##### The Freedom Wrapper Project was created for a multitude of reasons:

- First, the barrier for application development on Android should be small. Android applications are an easy way to get custom-made platforms tailored to your individual needs. [Android Studio](https://developer.android.com/studio/intro) is an extremely robust tool-set and it is well-suited to make anyone a developer with little effort. No one should rely on others for those needs when possible. Sometimes coding for your first time can be overwhelming when there isn’t enough positive feedback to keep you going. Every roadblock seems like a mountain and one line of red code can wreck havoc on your psyche. While web guides are an excellent source, there are thousands of them. People have to sift through them, find which ones actually work for their needs, and the guides still leave a lot to be desired when it comes to actually creating an original or purposeful application. This leaves individuals without “coding skills” at the behest of individuals, corporations, and governments to provide them with mobile applications that are generally a one-size-fits-all approach.

- This leads us to the second reason for this project: security. Android applications on the market are inundated with in-app purchases for extra content, ads with cross-site tracking capability, and permissions that seem mostly unnecessary for the average user. While Google has done a good job attempting to solve these permission problems recently, there is still concern. Sometimes is feels like Android applications are just a more robust way to collect your data for monetary or insidious gain. The Freedom Wrapper Project was created on the idea that security and privacy should be simple, cheap, and effective. Most mobile websites are already works of art. A mobile application seems like a complex, expensive, and ineffective solution for some users that just want to get on an application, use it safely, and get off of it soon-thereafter. Mobile browsers aren’t much better. Browsers are excellent tools to keep you browsing websites within the same application ecosystem. However, this can cause some fundamental security concerns. What happens when a website you visit is malicious? The entire browser, while sand-boxed, is compromised nonetheless. This means everything you search afterwards is potentially compromised. This is not to say all mobile browsers are bad. Many mobile browsers sandbox each individual browsing tab, protecting you in each tab sub-process. The original tab, however, will likely be a problem until you close it – and you won’t know if it is actually compromised until much, much later. While this situation may be unrealistic, it does happen and it has been documented. In fact, sometimes all the bells and whistles you associate with mobile browsers can be a security death knell. For instance, it came out this year (2020) that Firefox Mobile had a [security vulnerability](https://thehackernews.com/2020/09/firefox-android-wifi-hacking.html) that has since been patched. While Android’s `WebView` may not be any better than Firefox Mobile at zero-day exploits, at least you know only one website and its data is compromised instead of an entire browsing session of compromised data. Furthermore, mobile browsers are (intentionally or not) data collection machines. Many mobile browsers, even with sandboxes and security measures, cannot and do not prevent cross-site tracking. Every time you open a new tab in the same mobile browser at the same time you are creating a unique browser fingerprint that can be used to associate, triangulate, and eventual track your online presence through that session. Mobile browsers are also entirely inconvenient if you have to close them multiple times a day just to gain a modicum of privacy. The Freedom Wrapper Project acts like an isolated, web-page specific browser. It is sand-boxed, like all Android applications. But, it can easily be deleted and reinstalled because you can make and remake the code at anytime on your own. Furthermore, The Freedom Wrapper Project isolates you from the Android ecosystem generally and prevents cross-site tracking through an isolated session approach. You are only going to one website at a time and so the problematic inheritance of multiple tabs cannot be used to track each individual browsing session accordingly. Hopefully, you are using The Freedom Wrapper Project with a trusted website. This will make it almost impossible for you to load malicious code onto it. Furthermore, the decentralized process of making the application yourself ensures you cannot be duped into installing an application that is really a malicious piece of software. It’s a security win-win-win. 

- Thirdly, The Freedom Wrapper Project is open source and completely free. Being open source allows one to scrutinize the code. However, scrutiny is important but not entirely valuable in and of itself. The Freedom Wrapper Project falls under an MIT License. This means you can use this code for personal or commercial use, making you only a few steps away from developing your own application. The fact that it is open source means you can mention that your app uses source code associated with The Freedom Wrapper Project in application store submissions and customers can vet it, follow it, and potentially use it to make their own applications. This sets a standard for application security practices that people can rely on when choosing to install your application and eventually others. While the MIT License gives you the ability to create commercial applications (that is, for profit applications), it is not the design and purpose of this project or this license to allow you to use advertisements on any application you make with The Freedom Wrapper Project source code. I do not condone the use of ads or allow the use of advertisements on any of The Freedom Wrapper Project based applications. If code is open but not free, it is useless to enhancing the experience of fellow technologists – whether in a security, privacy, or creative context. This is why almost all app developers feel the need to load their applications with advertisements instead of content or useful code that makes our lives better. Don’t be the kind of developer that loads their application with advertisements. 

##### The following is a guide on how to get set up with The Freedom Wrapper Project so you can officially make your own application!

### For Newbloods:

1. First things first. You’ll need to install Android Studio on your computer. Head over to this website to download and install it: [Android Studio Download](https://developer.android.com/studio). 

2. Now, you’ll need to download The Freedom Wrapper Project Repository to your computer. The easiest method will be to download the master archive located here: [The Freedom Wrapper Project Download](https://github.com/mdbench/The-Freedom-Wrapper-Project/archive/master.zip). Once downloaded, head to the folder where you downloaded it and unzip or extract the file. This is usually as easy as right clicking the file and going to the button that says: **“Extract here”** or **“Unzip.”** It will take a couple of seconds for it to extract. In the file that is extracted, you should see all of the available applications The Freedom Wrapper Project has pre-made, along with the original source code dubbed **”The Freedom Wrapper Project”**. 

3. Next, open up Android Studio (if you already haven’t). It will show you a prompt that says open or make a new project. Click the **“Open”** button. Use the file browser to navigate to the folder where you downloaded The Freedom Wrapper Project master archive and click on the folder with the green android/alien where it says “The Freedom Wrapper Project.” It’ll take a few seconds to a minute to load depending on your computer. 

4. On the left-hand side there is a button that says “Project.” It is right next to the “ResourceManager” button. I promise it is there. There are a lot of buttons on Android Studio so give yourself some time to adjust and don’t feel overwhelmed. Once opened, you should see some folders with folder trees. Click on the sideways triangle (it honestly looks like a video play button) to open up a folder’s tree. It will expand or close each time you click it. The first file you will need to modify is in the folder labeled “java.” Go to **com.matthewbenchimol.thefreedomwrapperproject** and click the sideways triangle (play button) again. Now, double click on the file that says: **“MainActivity.”** Go down to the *48th* line of code where it says `webView.loadUrl(“https://wikipedia.org”)` and replace the https://wikipedia.org with the website you are trying to “wrap”. Make sure you keep the `“ ”` surrounding the website or the build will not compile! For example, let’s say you want to create a wrapper for Facebook. You would place https://facebook.com where the Wikipedia link is and the product would look like this: `webView.loadUrl(“https://facebook.com”)`. I have provided comments on the various lines of code should you be interested in turning on or off certain aspects of the application that are preset. I highly suggest you leave them as is unless you know what you are doing. 

**That’s it! That is technically all you have to do to create your first application. There are additional network security settings I highly suggest. These are not specifically necessary. If you want the extra security (you do), continue below. Otherwise, skip the fifth and sixth steps.**

5. Open the “Project” button again if for some reason you or Android Studio toggled it close. This time go to the folder that says **“res.”** Click the sideways triangle to open up the folder tree. Then, click on the sideways triangle for two folders to expand the folder tree. One is called **“xml”** and one is called **“raw.”** Open the browser of your choice. For example, **Chrome, or Firefox.** Go to the website you are trying to “wrap.” Sticking with the Facebook example above, go to https://facebook.com.

- For Firefox: Once the page is loaded, click on the padlock next to the website in the navigation bar. Click on the arrow that says **“Connection secure”** and click **“More Information.”** This will open up a page security tab. Once that is opened, click on the button that says **“View Certificate.”** It will open a page where you can export certificates. Click on the certificate tab to the farthest right and scroll down to where it says download. Click the **“PEM (cert)”** option. Save the certificate to the folder we opened earlier in **“res”** labeled **“raw.”**

- For Chrome: Once the page is loaded, click on the padlock next to the website in the navigation bar. Click on the tab that says **“Certificate (Valid).”** Click on the tab that says **“Details.”** Go to the certificate hierarchy and click on the certificate that has **“Builtin Object Token:”** next to it. Go to the button on the bottom right that says **“Export.”** Save the certificate to the folder we opened earlier in **“res”** labeled **“raw.”**

6. Now, go back to Android Studio and open the **“xml”** folder tree we discussed in *Step 5* and double click on the file that says **“network_security_config.”* Follow the directions that are listed as code comments. They should start like this: `// this is a network security configuration`. For future reference, all java code comments start with // and are grayed out.

7. Lastly, go to the top of Android Studio where the drop-downs are and click on the “Build” drop-down next to “Refactor” and “Run.” Then, click “Generate Signed Bundle / APK…” and follow the prompts. Make sure you click on the .apk button when creating your application. The app bundle (.aab) is strictly for the Google Play Store and will not be install-able on your Android phone. It is meant for Google Play Store Submissions. You will also be prompted to create a signing key. Please make sure you make one. This is important: a signing key let’s everyone know the application is legitimate and gives users the ability to verify it accordingly. You can fill anything you want for the signing key. I suggest you add the minimum: First and Last Name (Your Name – as this is *your* application), Organization (The Freedom Wrapper Project), and add a password that is yours and yours alone. After that, you can just press the **“Next”** button. Then, click the **“V1”** and **“V2”** check boxes and highlight the **“Build Variant”** that says **“Release.”** It will start the build process. 

8. There should be a notification that pops up after you have successfully built the application. It will say “locate” on it. Click it and Android Studio will automatically open the folder containing your recently developed application. Copy the .apk file it created to a folder that will let you find it easily now and in the future, change the name of the file (while preserving the .apk file tag at the end of it), download it to your phone through a USB (preference) or by uploading it to the cloud. Install it and ignore the warning about “installing from unknown sources.” You made this app so you can guarantee it is not malicious. Open it when it is finished installing on your Android Device. **Congratulations! You are now using The Freedom Wrapper Project.**
