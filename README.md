# Grappl

![django-large](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/django-large.png)
![cover](https://github.com/Blaiski/Grappl/images/Screen Shot 2023-06-19 at 10.16.15 AM.png)

## Did you know that up to 50% of developers' time is spent understanding existing code?
Welcome, developers! Tired of wasting precious time searching for that elusive piece of code? Frustrated with the challenges of understanding code impact and communicating it effectively to your team? Say hello to Grappl, your ultimate coding companion!


## Addressing Developer's Pain Points
Grappl was designed with one goal in mind: to alleviate developers' most nagging pain points. We understand the struggles you face daily, such as:
• Figuring out what a piece of code does
• Locating the exact location of a feature or bug fix in your codebase
• Identifying potential breakages caused by a single code change.

## Unveiling the Invisible City of Code
Imagine having a live Airview™ of your codebase, providing a visual landscape of your project. With Grappl's codebase visualization feature, you gain an unprecedented understanding of your developers' work. Spot early signs of code degradation and take action before things spiral out of control. Exciting developments await!


## Feature Highlights That Will Revolutionize Your Workflow
### Live Dashboard Integration
Access your development issues where you need them most, without unnecessary frills. Seamlessly connect to Jira, Trello, and more (additional board services coming soon!). Perform common actions directly from your development environment, streamlining your workflow.

### Codelink™ 
Instantly locate the code items you need to modify or fix. Grappl empowers you with meaningful domain knowledge right within your source code. Effortlessly navigate through design and code dependencies like a pro. Say goodbye to knowledge loss with Grappl's automated knowledge capturing.

### Airview™
Unleash the power of intuitive codebase exploration, without getting lost in technical details. Gain insights into how each feature or bug fix impacts your codebase. Unravel hidden design insights that were previously invisible. Prepare for even more exciting features on the horizon!


## Preview Version
Be among the first to discover the capabilities of Grappl! This preview version marks our debut on the VS Code marketplace. We are thrilled to offer you early access to Grappl. Explore it, provide feedback, and let us know what you think. Go ahead check it out... and drop us a line on any of [our channels](#bugs--feature-requests)! Please see [License](#license) for important details.




## Bugs & Feature Requests
- To report bugs or propose new features, please use our [Github issue page](https://github.com/Blaiski/Grappl/issues).
- To see what other users think of Grappl, visit our community [discussion page](https://grappl.io/community/).
- You can also reach us on our [Q&A](https://marketplace.visualstudio.com/items?itemName=grappl.grappl&ssr=false#qna) section on vscode marketplace.
- Or simply write us on [grappl.vscode@gmail.com](mailto:grappl.vscode@gmail.com).


---

## Quick Start 

### Step 1—Parsing of your Workspace
When you open a workspace, Grappl will run a background process to parse your codebase and build a model of its contents. This normally takes less than a minute, however it would vary depending on the number of files you have and the languages they are in.

💡 By default, only contents in your `src` folder are processed. You can add more folders in user settings<sup>‡</sup>.
![](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/folderConfig2.png)

💡 If you want to include all folders under your workspace, then you can use the following configuration<sup>‡</sup>. ![](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/folderConfig.png)

🛑 If you need to stop the parsing for any reason, simply hit: `alt+c`.

Once the parsing is complete, any changes to your code are reflected in the model instantly, so it is kept up to date all the time.


### Step 2—’Seeing’ your Codebase for the first time

This will be so fun! Grab a cup of ☕️ and prepare to catch the first sight of your codebase landscape 🏙!

💡 Hit `alt+v` to see your codebase coming to life!
![](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/Grappl_Vis.png)

### Step 3—Explore your new city

Give it a go, use your mouse or trackpad to move around your 3D codebase, just like you’d do in a PC game. You can also use the `arrow keys` to **pan** in either of the four directions, or `cmd+arrow keys` to **rotate** around. If using a trackpad, use `two fingers` to pan around.

Here’s a quick key map to help you interpret the visualisation. The size of buildings will give you indication of how complex that component is.
![mapping](https://raw.githubusercontent.com/Blaiski/Grappl/a7d7e3106d6feda642e6a73da11d626636da6d80/Mappings/Mappings%20Dark%20Mode.png)

🧪 You can play around a bit with how things are mapped by changing your user settings (hit `alt+v` again for changes to be reflected)
![mappingPrim2](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/MappingPrim2.png)
![mappingMeth](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/mappingMeth.png)


### Step 4——Seamless Integration with Dashboard Services

Connect Grappl to your favorite dashboard services such as Jira and Trello (with more options on the way!). Hit alt+d to establish the connection effortlessly. Grappl Explorer will display your boards and their relevant contents, ensuring you have all the information you need at your fingertips.


	💡 To connect to a dashboard service, hit `alt+d` !
![d](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/connectDash2.png)


🧪 **Explore the Test Board**

For a quick start, we have created a public Trello testing board with sample data. Check it out at https://trello.com/b/s1PUl0IO.
![](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/DashNew.png)
 
Feel free to either join in, or [copy it as a private board to your own account](https://support.atlassian.com/trello/docs/copying-cards-lists-or-boards/#:~:text=of%20its%20cards.-,Boards,-You%20can%20even)! 

💡 Grappl will automatically detect and recognize your development columns and cards on a Trello board as long as their names follow common agile practices in the industry.
Once you connect to a board service, Grappl Explorer will display your boards and their relevant contents.

![](https://github.com/Blaiski/Grappl/blob/main/images/gifs/Jira%20Auth.gif?raw=true)


### Step 5-Automated Card Checkout/Checkin with Codelink™️
1. Once you have connected your preferred board service, Grappl Explorer will display all your active issues, tasks, and more.
2. Select the card you want to work on and simply press alt+c to check it out.
3. Now, start working as you normally would. When you're ready to commit your changes, Grappl will automatically detect your code item contributions or modifications and prompt you.
4. If you accept, Grappl will initiate the three-legged Codelink™️ process, handling everything seamlessly.
5.Watch the magic happen! Grappl will create links, commit your staged changes, update your card on the board service, and even add helpful annotations to your code items (don't worry, you can disable them in an upcoming release).
(Note: You'll still have the opportunity to edit your commit message and other details before pushing.)
Experience the power of automated card checkout/checkin with Grappl, simplifying your workflow and saving you time. 
5. _(Note: You'll still have the opportunity to edit your commit message and other details before pushing.)_


**Flexibility at your fingertips!** With Grappl, you have complete control over the code items you want to link. Don't feel obligated to link every single code item you've changed. Select only the ones that matter to you and leave the rest behind.

**Forgot to check out a card before diving into your work?** No worries! You can check out a card at any time before committing your changes. Adjust the timespent for your worklog entry to ensure accurate tracking.

**Already committed your changes?**  There's still a solution! Simply navigate to the card you've been working on and press `alt+L`. A prompt will appear, allowing you to select the specific code items you want to link. Hit enter, and now you have the option to **amend** your latest commit. Grappl gives you the flexibility to adapt to any situation and maintain a seamless workflow.
![cardCheckout](https://github.com/Blaiski/Grappl/blob/main/images/gifs/card%20checkout.gif?raw=true)
![codelink](https://github.com/Blaiski/Grappl/blob/main/images/gifs/codelinking.gif?raw=true)


### Step 6—Find What You Need, Faster
With Grappl's code-item and design-item linking, pinpoint exactly what each code item does and visualize its impact on the codebase. Seamlessly navigate between code and design elements. Unleash the power of code impact visualization, all in real-time. No more manual digging through commits—Grappl has your back!


1. Explore the connections! After making changes to a code item, simply point to it and press `alt+r`. Witness the magic as Grappl reveals the _Related Design Items_. Gain valuable insights into the broader context of your code changes.
2. Dive deeper into the code-card relationship. Direct your attention to the card you've been working on and press alt+r. Grappl will display the _Related Code Items_, illuminating the specific code components tied to the card.
3. **Unveil the power of visualization!** Activate the code impact visualizer by selecting your card and pressing alt+i. Watch as Grappl presents the _Code Impact Visualisation_, providing a visual representation of your changes across the entire codebase. See the bigger picture in a glance!
4. Real-time synchronization for seamless collaboration. Grappl operates in real-time, ensuring that everything remains synced with your board service and repository. Stay up-to-date with the changes made by your team members, instantly reflected in your workspace.
5. Bid farewell to manual digging. No more searching through endless commit threads and changeblobs. Grappl empowers you to navigate and comprehend code changes effortlessly, saving you time and effort. Say goodbye to the tedious manual tasks and embrace a streamlined development experience.


![advantages1](https://github.com/Blaiski/Grappl/blob/main/images/gifs/advantages1.gif?raw=true)
![advantages2](https://github.com/Blaiski/Grappl/blob/main/images/gifs/vis3.gif?raw=true)


---
‡ <sup>Exercise caution when utilizing the '**' feature as it is currently in the experimental phase. Its usage may lead to prolonged parsing time, particularly if your workspace folder contains numerous subfolders with an extensive number of files, such as a 'node_modules' directory.</sup>

### Terminologies
▸ **Code Item:** Methods, functions, namespaces, and more—any component at the code level.

‣ **Design Item:** Issues, bugs, features, and other actionable items on your board.

‣ **Codelink:** Codelink is Grappl's powerful and automated code-to-design-to-commit linking operation. It establishes a connection between your code items, design items, and commit changeblob, forming a three-legged process. By linking your code-item-level source code changes to the corresponding design item you've been working on and your commit changeblob, Codelink streamlines your workflow. It goes beyond linking and updating your card on the dashboard service, automatically adding worklog entries, timespent, and even GitHub permalinks. In upcoming releases, you'll also have the option to annotate your code items with the design item key. With Codelink, Grappl ensures seamless synchronization with your remote repository, keeping everything up to date and enhancing your development process.<sup>†</sup>.



---
† <sup>Only Githup is supported at the moment, we have Bitbucket and others coming up down the line.</sup>


## Request a Demo
Curious to see how Grappl can revolutionize your organization or team's development experience? Reach out to us at [grappl.vscode@gmail.com](mailto:grappl.vscode@gmail.com) to request a personalized demo. We'll be delighted to arrange one for you! We will be happy or arrange one!

## Reviews & Ratings
If you've had a positive experience with Grappl, we kindly ask you to share your feedback on the [Rating & Review](https://marketplace.visualstudio.com/items?itemName=grappl.grappl&ssr=false#review-details) section on the marketplace. Your reviews help us spread the word and continue improving Grappl for developers like you. Thank you!

➜ **UPDATE | 15Aug, 2023:** Now you can also rate us privately and anonymously! Simply hit the keyboard chords `alt+f alt+f` (twice in sequence).

![rateUs](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/rateUs.png) 


## Grappl's Visualization Showcase — _Explore Popular Codebases: Delve into the world of open-source projects visualized by Grappl_


### Vscode [repo](https://github.com/microsoft/vscode)
![vscode](https://user-images.githubusercontent.com/31612240/178550039-61cfc5ad-39b0-4f53-b838-36589f193b22.png)
![vscode](https://user-images.githubusercontent.com/31612240/178550223-afea3b41-f776-4044-b157-580a2cc4b541.png)

### ASP.NET Boilerplate [repo](https://github.com/aspnetboilerplate/aspnetboilerplate) 
![aspnetboilerplate](https://blaiski.github.io/agileInsight.page/screenshots/ASP.NETBoilerplate.png)

### Django Lib [repo](https://github.com/django/django)
![django](https://blaiski.github.io/agileInsight.page/screenshots/django.png)
![django](https://user-images.githubusercontent.com/31612240/178551764-7001dc33-785b-466d-aef2-3b9cd59ebfb1.png)

### Amazon Web Services SDK for Go Language | [repo](https://github.com/aws/aws-sdk-go)
![awsgo](https://user-images.githubusercontent.com/31612240/178552902-d4aed912-902b-4b5b-82fe-277e6bf8d3e6.png)
![awsgo](https://user-images.githubusercontent.com/31612240/178552877-a4c469ef-bc67-4925-952a-097c4715ccbc.png)


### Facebook’s React API [repo](https://github.com/facebook/react)
![react](https://user-images.githubusercontent.com/31612240/178526387-9bd3b41e-424c-442c-b6ca-1eae95d6b6d6.png)


### Keras Lib [repo](https://github.com/keras-team/keras)
![keras](https://user-images.githubusercontent.com/31612240/178524511-7deb8ea5-ab7c-4f7e-befc-254666c51e36.png)

### Facebook iOS SDK | [repo](https://github.com/facebook/facebook-ios-sdk) 
![ios](https://user-images.githubusercontent.com/31612240/178552438-c797bee2-4e7a-49bd-9fc6-070e5e0bafad.png)
![ios](https://user-images.githubusercontent.com/31612240/178552499-d17b330c-2681-4871-8c3c-b1ecec75d687.png)

## Your Privacy Is Our Priority
Rest assured, Grappl does not store any personal information or project data. All processing occurs within your own environment, and data is fetched live from authenticated board services without caching. We prioritize your privacy and data security. 

## Telemetry
Grappl uses VS Code's official and approved Telemetry Module, along with Azure's Application Insights. This ensures that your privacy is strictly respected, that only minimal application usage data is sent, and that it is done completely anonymously. We use approved telemtry module to help us improve Grappl and keep rolling out relevant features. If you wish, you may change your telemetry level (`telemetry.telemetryLevel`) in user settings.


---

## License
Our license and Terms of Use can be found [here](https://marketplace.visualstudio.com/items/grappl.grappl/license).

Grappl is commercial software, and comes also with a standard package available to use for all, free of charge. This **preview version** of Grappl is offered as a free trial, and will expire on `29th Dec, 2023`. Our free standard version will then subsequently replace it. 


`Note:` Some premium features in the preview version may not be available in the free standard package. 

---


✴️We extend our grattitude to [AUT Ventures](https://ventures.aut.ac.nz) for their invaluable support and incubation of innovation.
