---
title: "Rules"
weight: 4

---

Business rules are what makes Kianda forms come alive. They represent the actual actions users intend to perform when they interact with form components. There are 59 rules you can apply to forms, see [Rules list](#rules-list).

There are two key principles to consider when working with forms:

1. Rule design - what type of rule you are going to apply and where, for example to a button, field or form

2. Rule order - if there are several rules attached to an item like a button, then the order of execution is important and can be modified to suit your needs.

   

## How to get started ##

If you go to **Administration** > **Designer** and click on a process or create a new process, the predefined rules are found in the left-hand pane under **Add a rule**.

![Rules](images/rulesgeneral.png) 

There are 10 categories of rules:

1. **Workflow** - rules that represent the actions a user intends to perform, when they interact with form components. There are 6 workflow rules, see [Workflow](workflow.md) for more information.
2. **Communications** - rules associated with user communication for example sending an email or triggering a user alert. There are 4 communication rules, see [Communications](communications/README.md) for more information. 
3. **Data** - rules associated with database operations like create, update and delete. There are 5 data rules, see [Data](data/README.md) for more information.
4. **Users** - rules associated with user properties, allowing user lookup or update a user. There are 4 user rules, see [Users](users/README.md) for more information. 
5. **File management** - rules concerned with generating documents such as Word, Excel or converting to PDF. There are 7 file management rules, see [File Management](files/README.md) for more information. 
6. **Tables** - rules associated with table operations such as updating, adding and removing table rows. There are 12 table rules, see [Tables](tables/README.md) for more information. 
7. **Dates** - date rules to calculate time and format dates. There are 4 date rules, see [Dates](dates/README.md) for more information. 
8. **Form actions** - rules linked to actions that are part of forms, for example submit, close or save. There are 6 form rules, see [Form actions](form_actions/README.md) for more information. 
9. **SharePoint** - SharePoint associated rules such as adding, finding or removing users. There are 10 SharePoint rules, see [SharePoint](sharepoint/README.md) for more information. 
10. **KiandaAI** - there is 1 KiandaAI rule related to text analysis, see [KiandaAI](kianda/kianda_ai.md) for more information. 



## When to use rules

You can add rules:

- [x] to a field
- [x] to a form 
- [x] to a process (the rule will run on load)



### Rule design ###

1. Click on an existing process by going to **Administration** > **Designer** and decide which form or field you will apply the rule to, by clicking on that item so that it is in **edit mode** so you can see the Pen button,  **Pen** button ![Pen button](C:\Kianda\docs-dev\rules\Readme2.assets\penicon.png) for example a form Training Approval or Submit button.

   ![Edit mode for forms and fields](images/formvsbutton.png) 

2. Click on **Add a rule** in the right-hand pane and click on a category of choice, such as **Communications** and then a rule **User alert**.

 



### Rule order ###

If there is more than 1 rule for an item like a field or button, then the order of execution must be considered. 

For example for a Submit button on a form I may want my **Send email rule** to be executed first before any other rule is executed. To do this click on the **Submit** button to make sure you are in **Edit** mode, and under **Rules** in the right-hand pane,  drag the **Send email** rule to the top of the list by clicking on the rule and dragging it to the top.

<img src="images/ruleorder.png" alt="Rule order" style="zoom:70%;" />



## Rules list ##

A full list of rules is available in the table below.

![Rules list](images/rulestable_orig.png)
