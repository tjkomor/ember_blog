<!-- A particular technical problem that you encounter and how you solved it (or your efforts to solve it, if you didn't end up solving it)
A post-mortum on what went well and what you would improve upon if you were to continue working on this project or if you started over --> -->

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

There were a ton of technical difficulties during this project. I think the main issue was strictly just the learning curve and lack of familiarity with Ember and Electron. But one issue that I really had trouble with was the implementation of the search bar. So ideally, when you search for a note, the note will only show up if what you enter in the search bar is included in the title of the note. I really had a tough time visualizing how all the different parts of the program were working together to make this happen.
