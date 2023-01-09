# namaste-react-question-answer

Lesson 1

**1.What is diference between React and ReactDOM ?**

The react package holds the react source for components, state, props and all the code that is react.

The react-dom package as the name implies is the glue between React and the DOM. Often, you will only use it for one single thing: mounting your application to the index.html file with ReactDOM.render().

The reason React and ReactDOM were split into two libraries was due to the arrival of React Native (A react platform for mobile development).

React components are such a great way to organize UI that it has now spread to mobile to react is used in web and in mobile. react-dom is used only in web apps.

**2.Why is React known as React?**

React was developed for applications (Facebook) that have constantly changing data. Since React is a front-end framework or the “View” in MVC, this means that as the user clicks around and changes the app’s data, the view should “react” or change with those user events. User events being mouse clicks, typing, submitting a form.

**3.What is CDN? Why do we use it?**

A content delivery network (CDN) refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content.

A CDN allows for the quick transfer of assets needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos. The popularity of CDN services continues to grow, and today the majority of web traffic is served through CDNs, including traffic from major sites like Facebook, Netflix, and Amazon.

A properly configured CDN may also help protect websites against some common malicious attacks, such as Distributed Denial of Service (DDOS) attacks.

**4.What is crossorigin in script tag?**

The crossorigin attribute sets the mode of the request to an HTTP CORS Request.
Web pages often make requests to load resources on other servers. Here is where CORS comes in.
A cross-origin request is a request for a resource (e.g. style sheets, iframes, images, fonts, or scripts) from another domain.

**5.What is async and defer?**

async - The browser will download the script file and continue parsing HTML parallelly until the file is downloaded. The file is executed as soon as it is downloaded.

defer - The browser will download the script and do HTML parsing at the same time. After parsing is done, the script files are executed in the order of their occurrence.

**6.What is Emmet?**

Emmet is a plug in for many popular text editors which greatly improves HTML & CSS workflow.

**7.What is difference between react.development.js and react.production.js files via CDN?**

The development build is used - as the name suggests - for development reasons. You have Source Maps, debugging and often times hot reloading ability in those builds.

The production build, on the other hand, runs in production mode which means this is the code running on your client's machine. The production build runs uglify and builds your source files into one or multiple minimized files. It also extracts CSS and images and of course any other sources you're loading with Webpack. There's also no hot reloading included. Source Maps might be included as separate files depending on your webpack devtool settings.

What specifically separates production from development is dependent on your preferences and requirements, which means it pretty much depends on what you write in your Webpack configuration.

**8.What is diference between React and ReactDOM?**

React library is responsible for creating views and ReactDOM library is responsible to actually render UI in the browser.This two was separated since react was lunch for mobile (react nativ) as  well.

_______________________
Lesson 4
_______________________

1.Is Jsx mandatory for React?
No. You can use  React.createElement("div",{id:"root"},"Hello World");

2.Is ES5 mandatory for React?
No. You can use other lower version as well.

3. {TitleComponent} vs <TitleComponent/> vs <TitleComponent></TitleComponent> in JSX
First Title component is Variable place holder and other two are functional component. Last two are same one is just self closing.

4.How can I write comments in JSX?
In JSX you can comment exactly like JavaScript withing {}.
const commentedCode=()=>{
  return (
    <>
      <div>Hello World<div>
      {//This is single line comment}
      {
        /*This
        is multiline
        comments
        */
      }
    <>
};

5.What is <React.Fragment></React.Fragment> and <></> ?
Both are same,second one is just shorter way to write it.
A common pattern in React is for a component to return multiple elements. Fragments let you group a list of children without adding extra nodes(like div) to the DOM.

