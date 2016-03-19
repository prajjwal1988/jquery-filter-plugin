# Jquery Filter Plugin

jQuery Filter plugin is my attempt at making a simple in-page filter plugin, it is very helpful where the user has an input textbox and a list of items.

Here is a simple step by step tutorial to use this plugin.

The most common scenario when we require a filter plugin like this is when we have a list of items on our page and we have a search box. A we type in the search box, the relevant matching items are displayed while the non-matching items disappear.

The items should be present inside a wrapper, and each of the items must have a specific class.  
The contents like title or fields that should be taken into consideration need to be wrapped inside an html element like 'span' with a class.

## Walkthrough of the Demo

In my example demo, there is a list of institutes which is wrapped inside a div with id="institutes_list"

Each institute inside the wrapper has a class "list-card". It has important fields like:

1.  Name of the Institute : With the class "card-title".
2.  Address of the Institute : With the class "address".
3.  Subjects that are taught in the Institute : With the class "subject_badge".

Now, We need to search based on all the above 3 fields in the items. To do this, we will create the search box in the folowing way : `<input type="text" class=" jquery_filter " placeholder="Search for Institute" data-search-items-wrapper-id="#institutes_list" data-search-item-class=".list-card" data-search-classes=".card-title,.address,.subject_badge">` 

The search box has the class **jquery_filter**  
Let us look at the attributes required here:  

1.  **data-search-items-wrapper-id** : This is the id of the wrapper of the items. In this case it is : **#institutes_list**
2.  **data-search-item-class** : The class of each item. In this case it is : **.list-card**
3.  **data-search-classes** : Comma separated classes that needs to be searched. In this case it is : **.title** , **.address** and **.subject_badge**

Please go through the code of the demo, I have provided a lot of comments to help you understand the code.