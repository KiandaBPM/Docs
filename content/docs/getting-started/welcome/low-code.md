---
title: "What is Low-Code Development?"
linkTitle: "What is low-code?"
weight: 3
typora-root-url: ..\..\..\..\static
---

Low-code development offers **software developers** a shortcut to create something new and beneficial for their organisation. Rather than thinking about every single line of code, as a developer you can take advantage of Kianda's **Developer** to create your own custom widgets from predefined field, rule and dashboard code.

You can also quickly use Kianda **Developer** to add [webhooks](#webhooks) providing an efficient way to push GET requests to other applications in real-time as the Kianda process runs, avoiding the need to poll for data. 

Kianda uses EmberJS to build widgets, and in particular the Handlebars templating library to power the application's user interface, see [templating basics](#emberjs-templating-basics) below to get started.



## EmberJS templating basics

With Handlebars you can quickly build web applications that are made up of different components. Handlebar templates contain static HTML and dynamic content inside Handlebars expressions, which are summoned with double curly braces: {{ }}

Dynamic content inside a Handlebars expression is rendered with data-binding. This means if you update a property, your usage of that property in a template will be automatically updated to the latest value.

### Helpers 

Ember gives the ability to write your helpers, to bring a minimum of logic into Ember templating. For example, let's say you would like the ability to add a few numbers together, without needing to define a computed property everywhere you would like to do so.

***Helper example***

![Helpers](/images/write-our-own-helpers.png)

#### Conditionals

Statements like **if** and **unless** are implemented as built-in helpers. Helpers can be invoked three ways; inline invocation, nested invocation and block invocation. For more details, click on the following link: https://guides.emberjs.com/v2.18.0/templates/conditionals/.



## How to get started with Developer

Kianda **Developer** is user-friendly interface to create custom widgets in a few minutes. A custom widget could be a 'Field', 'Rule' or Dashboard widget', see example of how to create a field widget below.

***Creating a custom field widget***

<video width="100%" style="width:100%" controls>
    <source src="/videos/createwidget.mp4">
    Your browser does not support the video tag.
    </source>
</video>



To create custom widgets:

1. Go to the **Side menu** > **Administration** > **Developer**

2. Click on **New widget**.

3. Fill out the **Edit widget** dialog box, that is **Title**, **Unique Id** (which is autofilled from the title), **Widget Icon**, where you can select from hundreds of icons, and then **Widget type**. There are 3 options: **[Field](#field-widget)**, **[Rule](#rule-widget)** or **[Dashboard widget](#dashboard-widget)** click on each link for details. 

   ![Edit widget](/images/editwidget.gif)

4. Click on **OK** when complete.

5. Widgets created are visible in the main widget view. From here a widget can be edited by clicking on the **Pen** button  ![Pen button](/images/bluepen.png) deleted by clicking on the **Bin/Trash** button ![Bin button](/images/binicon.png) and earlier versions restored by clicking on the **Version restore** button ![Restore](/images/bluerestore.png).

   ***Widget view***

   ![Widget view](/images/widgetview.gif)

6. [Webhooks](#webhooks) can be created to send a message to a specific URL, by clicking on the **Webhooks** button, click on the link for more information.

   

### Field widget

When you create a custom field widget, the widget UI and widget code are available. The two images below display the default code for 'Widget UI' and 'Widget Code'.

The 'Widget UI' defines the HTML, handlers, expressions and more.

***Field widget UI***
![Widget UI](/images/widgetfieldui.gif)

The 'Widget Code' defines the logic and functions.

***Field widget code***

![Widget code](/images/widgetcodefield.png)

Created field widgets will be available for use in Kianda Designer by going to **Side menu** > **Administration** > **Designer** > **click on an existing process** or **Add new** to add a new process then click on a form to edit it, and see the Custom fields added under **Controls**.

![Custom fields](/images/customcontrol.png)



### Rule widget

The two images below display the default code for 'Widget UI' and 'Widget Code'.
The 'Widget UI' defines the HTML, handlers, expressions and values for rules. 

***Rule widget UI***
![Widget rule UI ](/images/rulewidgetcode.gif)

***Rule widget code***

The 'Widget Code' defines the logic, functions and variable routines.

![Widget rule ](/images/rulewidget.gif)

### Dashboard widget

The two images below display the default code for 'Widget UI' and 'Widget Code'.

The 'Widget UI' defines the widget configuration view, used for editing and the widget runtime view, or view mode. 

***Dashboard widget UI***

![Dashboard widget UI](/images/dashboardui.gif)

***Dashboard widget code***

![Dashboard widget code](/images/dashboardcode.gif)



### Webhooks

To create webhooks:

1. Click on the **Webhooks** button from the main widget view to add a webhook. 

![Webhooks](/images/webhooks50.gif)

2. Use the slider to turn on **Enable Created Callback**, **Enable Updated Callback**, **Enable Deleted Callback** and **type in the URL** in each case to respond to process instance create, update and deleted events. 

   For example choosing **Enable Created Callback** will enable a URL callback everything a process instance is updated. This results in a HTTP GET request with parameters instanceID={instanceID}, processName={processName} and eventType=created being issued to the give URL

   **Note:** Callback has a timeout of 10 seconds.

3. Click on the **Help** button ![Help button](/images/webhookhelp.png) for clarification. 

4. Click on **OK** when done.



### What's next  ![Idea icon](/images/18.png) ###

If you want to use Kianda for no-code development, then follow the steps below:

![1](/images/one.png)  [**Plan your process**](/docs/getting-started/create-first-process/plan-your-process/) 

![2](/images/two.png)  [**Design and build your process**](/docs/getting-started/create-first-process/design-and-build/)

![3](/images/three.png)  [**Publish your process**](/docs/getting-started/create-first-process/publish-your-process/)



### **To return to the previous pages click on the links below**  ![Idea icon](/images/10.png) 

- **[Getting started guide](/docs/getting-started/)**
- **[Welcome to Kianda](/docs/getting-started/welcome/)**
- [**What is no-code development**](/docs/getting-started/welcome/no-code/)
- [**Logging in to Kianda**](/docs/getting-started/logging-in/)
- [**Create your first Kianda process**](/docs/getting-started/create-first-process/)
- [**Controls**](/docs/getting-started/create-first-process/design-and-build/add-controls-and-rules/)
- [**Rules**](getting-started/create-first-process/rules.md)

