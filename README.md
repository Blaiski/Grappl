# Grappl for Visual Studio Code


## Did you know that up to 50% of developers' time is spent understanding existing code?
Welcome, developers! Tired of wasting precious time searching for that elusive piece of code? Frustrated with the challenges of understanding code impact and communicating it effectively to your team? Say hello to Grappl, your ultimate coding companion!
</br></br>

## Addressing Developer's Pain Points
Grappl was designed with one goal in mind: to alleviate developers' most nagging pain points. We understand the struggles you face daily, such as:
•	Figuring out what a piece of code does
•	Locating the exact location of a feature or bug fix in your codebase
•	Identifying potential breakages caused by a single code change.

## Unveiling the Invisible City of Code
Imagine having a live Airview™ of your codebase, providing a visual landscape of your project. With Grappl's codebase visualization feature, you gain an unprecedented understanding of your developers' work. Spot early signs of code degradation and take action before things spiral out of control. Exciting developments await!
</br></br>

## Feature Highlights That Will Revolutionize Your Workflow
### Live Dashboard Integration
Access your development issues where you need them most, without unnecessary frills. Seamlessly connect to Jira, Trello, and more (additional board services coming soon!). Perform common actions directly from your development environment, streamlining your workflow.

### Codelink™ 
Instantly locate the code items you need to modify or fix. Grappl empowers you with meaningful domain knowledge right within your source code. Effortlessly navigate through design and code dependencies like a pro. Say goodbye to knowledge loss with Grappl's automated knowledge capturing.

### Airview™
Unleash the power of intuitive codebase exploration, without getting lost in technical details. Gain insights into how each feature or bug fix impacts your codebase. Unravel hidden design insights that were previously invisible. Prepare for even more exciting features on the horizon!
</br></br>


## Preview & Pre-Release Version
Be among the first to discover the capabilities of Grappl! This pre-release version marks our debut on the VS Code marketplace. We are thrilled to offer you early access to Grappl. Explore it, provide feedback, and let us know what you think. Go ahead check it out... and drop us a line on any of [our channels](#bugs--feature-requests)! Please see [License](#license) for important details.
</br></br>



## Bugs & Feature Requests
- To report bugs or propose new features, please use our [Github issue page](https://github.com/Blaiski/Grappl/issues).
- To see what other users think of Grappl, visit our community [discussion page](https://grappl.io/community/).
- You can also reach us on our [Q&A](https://marketplace.visualstudio.com/items?itemName=grappl.grappl&ssr=false#qna) section on vscode marketplace.
- Or simply write us on [grappl.vscode@gmail.com](mailto:grappl.vscode@gmail.com).
</br></br>

---
</br>

## Quick Start 

### Step 1—Parsing of your Workspace
- When you open a workspace, Grappl will run a background process to parse your codebase and build a model of its contents. This normally takes less than a minute, however it would vary depending on the number of files you have and the languages they are in.

💡 By default, only contents in your `src` folder are processed. You can add more folders in user settings<sup>‡</sup>.
![](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/folderConfig2.png)

💡 If you want to include all folders under your workspace, then you can use the following configuration<sup>‡</sup>. ![](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/folderConfig.png)

🛑 If you need to stop the parsing for any reason, simply hit: `alt+c`.

Once the parsing is complete, any changes to your code are reflected in the model instantly, so it is kept up to date all the time.
</br></br>

### Step 2—’Seeing’ your Codebase for the first time

This will be so fun! Grab a cup of ☕️ and prepare to catch the first sight of your codebase landscape 🏙!

💡 Hit `alt+v` to see your codebase coming to life!
![](https://grappl.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F20f24173-d20f-42c0-9152-3ab4ea236284%2FScreen_Shot_2023-04-10_at_3.25.49_PM.png?id=edc6a51a-ee6c-4cfb-a756-b91a59b4f992&table=block&spaceId=a41b2efe-ad72-4b94-858c-f36d23046c2a&width=1060&userId=&cache=v2)

### Step 3—Explore your new city

Give it a go, use your mouse or trackpad to move around your 3D codebase, just like you’d do in a PC game. You can also use the `arrow keys` to **pan** in either of the four directions, or `cmd+arrow keys` to **rotate** around. If using a trackpad, use `two fingers` to pan around.

Here’s a quick key map to help you interpret the visualisation. The size of buildings will give you indication of how complex that component is.
![mapping](https://raw.githubusercontent.com/Blaiski/Grappl/a7d7e3106d6feda642e6a73da11d626636da6d80/Mappings/Mappings%20Dark%20Mode.png)

🧪 You can play around a bit with how things are mapped by changing your user settings (hit `alt+v` again for changes to be reflected)
![mappingPrim2](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/MappingPrim2.png)
![mappingMeth](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/mappingMeth.png)

</br>

### Step 4—Connect to a dashboard service

For now, Grappl can connect to your Jira Software or Trello boards. We have Asana, Linear, and others coming up down the line! 

	💡 To connect to a dashboard service, hit `alt+d` !
![d](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/connectDash2.png)

</br>

🧪 **Test Board Available**

To make things a bit faster, we created a public trello testing board with some data in it for you to get started. Here it’s: https://trello.com/b/s1PUl0IO.
![](https://raw.githubusercontent.com/Blaiski/Grappl/main/images/DashNew.png)
Feel free to either join in, or [copy it as a private board to your own account](https://support.atlassian.com/trello/docs/copying-cards-lists-or-boards/#:~:text=of%20its%20cards.-,Boards,-You%20can%20even)! 

💡 Grappl will automatically recognise your dev columns and cards on a Trello board as long as their naming follows common agile practice in industry. 

Once you connect to a board service, Grappl Explorer will display your boards and their relevant contents.

![](https://github.com/Blaiski/Grappl/blob/main/images/gifs/Jira%20Auth.gif?raw=true)
</br> 
</br></br>

### Step 5—Try out our automated card checkout/checkin process (includes automated three-legged Codelink™️)
1. After you have connected your chosen board service, Grappl Explorer will display all your active issues, tasks, etc. 
2. Select the card you want to work on and hit `alt+c` to check it out. 
3. Now, start working as usual. Once you stage your changes and are ready to commit, Grappl will detect all your code item contributions or changes and will show you a prompt. 
4. If you accept, it will initiate the three-legged Codelink™️ process and that’s it… you’re all done! 
5. Grappl will create some magic links, take care of committing your staged changes, update your card on the board service, and add helpful annotations to your code items (you will be able to turn these off in an upcoming release). 
5. _(Note: you will still get to edit your commit message and other stuff before things are pushed)_

**Don’t want to link all the code items you changed?** That’s fine, you can of course select which ones you want to be linked.

**Forgot to check out a card before you started working?** That’s all good, you can check out a card any time before you’ve committed your changes. You'll also get to edit the timespent for your worklog entry.

**You have already committed your changes?** There’s still a way around! Just head to the card you worked on, and hit `alt+L`. You will get a prompt and can now select all the code items that you want to link. Hit enter, and now you can choose to **amend** your latest commit!!
![cardCheckout](https://github.com/Blaiski/Grappl/blob/main/images/gifs/card%20checkout.gif?raw=true)
![codelink](https://github.com/Blaiski/Grappl/blob/main/images/gifs/codelinking.gif?raw=true)
</br>

### Step 6—Find what you looking for faster and navigate through your design-to-code dependencies intuitively
Now that your code items are linked up with your design items, you can point to any code item in your source code and tell exactly what it’s doing... and tell what design items its impacting! You can also point to any design item in Grappl explorer and be able to navigate directly to all the code items that are related to it! 

1. Try it out, point to any code item you just changed and hit `alt+r`. This will show _Related Design Items_!
2. Now point to the card that you just worked on, and similarly hit `alt+r`. This will show its _Related Code Items_
3. **You can also reveal things using the visualization.** Hit `alt+i` while your card is selected. This will trigger _Code Impact Visualisation_. Now you can visually see your changes across the entire codebase!
4. Grappl works in real-time, and keeps everything synced up with your board service and repository. This means changes done by other members of your team, will be instantly visible on your end too. 
5. Say no to manual digging through those endless commit threads and changeblobs.

![advantages1](https://github.com/Blaiski/Grappl/blob/main/images/gifs/advantages1.gif?raw=true)
![advantages2](https://github.com/Blaiski/Grappl/blob/main/images/gifs/vis3.gif?raw=true)

</br> 

</br>

---
‡ <sup>Be cautious when using '`**`' as it’s experimental for now and could result in long parsing time, especially when your workspace folder has subfolders with large number of file, e.g., a ‘node_modules’ one!</sup>
</br></br>

### Terminologies
▸ **Code Item:** A method, a function, a namespace, and the likes (including a file).

‣ **Design Item:** An issue, a bug, a feature, and the likes (any item on your board that you need to action).

‣ **Codelink:** Grappl's automated code-to-design-to-commit linking operation. It links your code-item-level source code changes to the design item you worked on, and to your commit changeblob. That's why we call it three-legged! Augmented with our Cardcheck out feature, it will update your card on your dashboard service (e.g., automatically add worklog entry, timespent, a Githup permalink, etc), annotate your code items with the design item key (optional in upcoming release), and sync everything up to your remote repository<sup>†</sup>.

</br>

---
† <sup>Only Githup is supported at the moment, we have Bitbucket and others coming up down the line.</sup>
</br></br>


## Request a Demo
To request a personalised demo to your organisation or team, please write us on [grappl.vscode@gmail.com](mailto:grappl.vscode@gmail.com). We will be happy or arrange one!
</br></br>

## Reviews & Ratings
If you use Grappl and like it, please consider reviewing it on the [Rating & Review](https://marketplace.visualstudio.com/items?itemName=grappl.grappl&ssr=false#review-details) section on the marketplace, and help us spread the word! Thank you! 
</br></br>

## Grappl's Visualization Showcase — _Popular open-source codebases as seen by Grappl_

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

## Privacy 
Grappl does not store any personal information or any data about your project or usage. All processing happens on your own environment, and relevant data are fetched live from authenticated board services on the fly without any caching or medium storage. 

---
</br>

## License
Our license and Terms of Use can be found [here](https://grappl.io/license). 

Grappl is a commercial software, and comes also with a standard package available to use for all, free of charge. This **preview version** of Grappl is offered as a free trial, and will expire on `29th Dec, 2023`. Our free standard version will then replace this preview version. 

`Note:` some features currently offered in this preview version are part of our premium package, and will not be available in the free standard package. 

---
</br>

✴︎ Kudos to [AUT Ventures](https://ventures.aut.ac.nz) for inccubating and supporting innovation 🥳
