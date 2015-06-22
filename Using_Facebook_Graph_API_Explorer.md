## Understanding the Facebook Social Graph

Facebook borrows terms from mathematical graph theory to describe features of its social graph model.

| **Feature**   | **Description** |
| ------------ | --------------- |
| **Node**     | An object within Facebook: a user, a photo, an event, etc.    |
| **Field**    | An attribute of a node: a user's birthday, the date of an event, etc. |
| **Edge**     | A connection between two nodes: a user's photos, a photo's comments, etc. |


## Using Graph API Explorer

The easiest way to experiment with Facebook Graph API calls in action is to use the Graph API Explorer, available at:

https://developers.facebook.com/tools/explorer/

You can issue RESTful API queries using the HTTP GET. POST, and DELETE commands that are available from the **Graph API drop-down menu**.

Queries you enter from the keyboard, or by selecting options provided by the Graph API Explorer interface, are displayed in the **Query field**.

Data returned from your query, or an associated error message, is displayed in the **Response text area** that occupies most of the right side of the window beneath the query field.   

![Facebook Graph API Explorer ](http://jkrick.com/markdown_image/graph_get_999.png)

Before you can issue a query, you will need to obtain an access token.

1. Click the **Get Token** button in the upper right corner of the Graph API Explorer interface.
2. Select **Get Access Token**.

![Facebook Graph API Explorer ](http://jkrick.com/markdown_image/graph_get_2.png)

>**Note**: When you build an actual application you will need to obtain an App Token to pass with your Login.

<ol start="3">
<li>The <strong>Select Permissions</strong> window displays. This pop-up lets you select additional fields to add to your query, but for this procedure we will leave all of the checkboxes unselected.</li>
<li>Click <strong>Get Access Token</strong>.</li>
</ol>

![Facebook Graph API Explorer ](http://jkrick.com/markdown_image/graph_get_11.png)

<ol start="5">
<li>A confirmation window appears that asks you to grant permission for the API call to return the selected information.</li>
<li>Click <strong>Okay</strong>.</li>
</ol>

![Facebook Graph API Explorer ](http://jkrick.com/markdown_image/graph_get_confirm_2.png)

>**Note**: In this query example, we are requesting information about the currently logged in user (shown as "me" in the query string. If we were querying against another user we would need to supply the users id and the user would receive a notification asking for permission to share information.

You can construct a query using Graph API Explorer's Query builder bar.

1. Search for a field name by entering text in the **Search** field, or add a field by selecting it from the drop-down list.

2. Click **Submit**.

![Facebook Graph API Explorer ](http://jkrick.com/markdown_image/graph_get_98.png)

<ol start="3">
<li>Note that the query returns only those fields that are selected in the Query builder bar.
</ol>

![Facebook Graph API Explorer ](http://jkrick.com/markdown_image/graph_get_33.png)