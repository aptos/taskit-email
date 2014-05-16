# Email Templates for TaskIT

## Instructions for Translators

English versions of each template are found in the 'en' folder. These are the 'originals' for reference and should not be edited. Each additional language has copies within the language folder. Those are the files that should be edited. Here's the current list of languages:

* Japanese: 'ja'

### Steps to Edit Templates

We are going to use the editor built in to github for our purposes. This is an online editor that allows us to instantly share updates. There is no software to download.

* Navigate to the file which you would like to edit by clicking the language folder, then the filename.
* Select 'Edit' from the tab menu displayed at the top of the file. The file should change to white text on a black background.
* You can now begin editing the file. It is ok to edit any text that is not part of the HTML or template markup. For example, template markup looks like this:

````erb
  <h2>Welcome to <%= site_name %>!</h2>
````

  In this case, only 'Welcome to' should be changed. However, if you would like to change the order of this greeting by placing the site_name before the welcome phrase, you may do that.

* Once your edits are complete, click the green "Commit changes" button near the bottom of the file.
* When you commit changes, you are welcome to add a comment below in the 'Commit changes' area, where some example text is shown.

### Viewing your changes

The github site doesn't have a simple way to show you how the HTML will look with one click, but there are two solutions that are pretty simple:


#### Use the GitHub HTMLPreview Bookmarklet tool

The quickest way to get a preview is to add a 'bookmarklet' to your bookmarks bar and preview the page right from github. A bookmarklet is a tiny javascript program that runs against the current page. So we'll create a bookmark, and instead of adding a normal URL, we'll paste in some javascript. Here's how to install it:

* Open the Bookmark Manager in Chrome. Bookmarks -> Bookmark Manager
* Click Bookmarks Bar
* RightClick under the list of bookmarks and 'Add Page...'
* Name: HTMLPreview
* URL:
````
 javascript:void(%27http://htmlpreview.github.io/%27%3D%3Dwindow.location%3Falert(%27Drag%20me%20to%20your%20bookmarks%20bar!%27):window.location%3D%27http://htmlpreview.github.io/%3F%27%2Bwindow.location)
````

To Preview the email, navigate to the template in Github and click 'Raw' in the github viewer menu. You'll see just the template contents. Then click your new 'HTMLPreview' bookmarklet. You should see the page re-rendered as a normal webpage.

Don't worry about the stuff like "<%= @setting.name %>", this will be filled when the application runs. In this case, the user's name will be substituted.

#### Save the file to your Desktop as '.html', then open them in your browser

* First, click the button labeled 'Raw' to see just our html page.
* Next, from the Chrome menu, save the file to your desktop: File -> Save Page As...
* When you save, remove the '.erb.txt' from the end of the file name, so that it ends in '.html'
* Now you can double click the file or drag it into your browser window.

Don't worry about the stuff like "<%= @setting.name %>", this will be filled when the application runs. In this case, the user's name will be substituted.

** It's possible that windows users will still see the markup. If this is the case, try the 'bookmarklet' approach**