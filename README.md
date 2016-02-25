What is Ember?

That's a great question, I'm glad you asked!

Ember is a JavaScript Web Framework that follows the standard MVC Framework(models-views-controllers). What makes Ember really cool is that it does alot for you. You are able to generate models, controllers, and components directly from the command line which is very similar to the Rails framework.

So now that we no a little bit about Ember, let's look at another technology, Electron.

Electron is a technology that allows you to build desktop applications. For example, if you successfully build an Electron app, you can use this app anytime you want, without internet connection. Electron actually combines Node.js and Chromium(Google Chrome) and enables you to build cross platform desktop applications. Something that is awesome about Electron is that amount of code(or lack there of) you need to write to create a fully functional application.

OK, so we've covered the basics. Let's dig a little deeper into these technologies.

Why would I want(or not want) to use Ember?

First off, Ember makes your life easier, at least a little bit.

Ember uses these things called Components which are extremely helpful, providing you actually know how to use them. A component is basically just a view that is totally isolated from the rest of the application. Basically, the component has no idea what is happening in the application, and it doesn't need to. You can actually reuse the same component throughout your application without touching the overall architecture of your code base.

One downside to Ember is that there is a very steep learning curve, at least there was for me. If you're considering building an application and have never used Ember before, it would benefit you to do as much research/practice with it as possible. I would guess that if you have worked with Angular or Backbone before, you might be able to pick up Ember fairly quickly, however, if the only framework you have ever work with is Rails(me), then I suggest you do some intensive research on the ins and outs of Ember.

So what's the deal with Electron?

Electron is so powerful because it lets you build desktop applications AND interact with the browser at the same time!

Electron has two main processes, the main process, and the renderer process. The main process create web pages by creating instances, and each instance is being run in its own rendered process. The renderer process basically just displays whatever the main process tells it to. So the renderer will go and ask the main process what it needs to display and then display it. This is what allows there to be communication between different web pages.

Technical Difficulties

There were a ton of technical difficulties during this project. I think the main issue was strictly just the learning curve and lack of familiarity with Ember and Electron. But one issue that I really had trouble with was the implementation of the search bar. So ideally, when you search for a note, the note will only show up if what you enter in the search bar is included in the title of the note. I really had a tough time visualizing how all the different parts of the program were working together to make this happen. It really didn't click for as to how these all of these moving parts were working together in order to render the notes that I was searching for. The first thing I tried to so was have an availableNotes method in my application.js file. After a lot of trial and error with this approach, I decided this just wasn't right way to go about this. The application file was creating and saving notes, and searching for a note isn't a part of CRUD functionality, so at this point I decided to ask my instructor for help. We ended up putting an availableNotes method in the components folder. I think it actually makes a lot of sense to pull this method out into its own component since it's only doing one thing. So in order to render this in our app, we need to go to the templates folder and write code that will render each availableNote. After going through that trial and error process, it was a lot more clear to me as to why we decided to write the code we did to render the searchable notes.

Moving Forward

My biggest issue with this project is that I just jumped right in. Usually, I feel like this is actually a good approach and I usually get a lot out of it. However, in this case, trying to jump right in with two different technologies was not the best idea. This was a recipe for instant frustration that ended up turning into a lot of compound frustration over a period of three days. If I were to restart this project I would definitely take the time to better understand the technologies I'm working with and how I need to use these technologies in order to produce the product that I want. I would also spend a lot more time reading the documentation for Ember. A large part of my frustration was that I needed to do a thing, but I didn't know how to write this in terms of code. When you are frustrated, the last thing you want to do is read the Ember documentation, but you have to. I think next time I'll spend some time reading the documentation before I even start the project just to get a better feel for what a given technology is capable of. Overall, I definitely learned some Ember and Electron, but I plan on redoing this project from scratch to solidify some of the basics that I still feel shaky on.
