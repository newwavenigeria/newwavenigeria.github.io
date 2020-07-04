# Usage

## Navigating to the Repository

After logging in, you'll see the default view. Click on the link indicated in the picture to get to the repository.

![Default Login View](https://i.imgur.com/BVkbTfl.png)

## Using the Repository

You'll then arrive at the repository, which contains all the code for the website. Below the picture is a table describing each file

![Repository View](https://i.imgur.com/0STzeuu.png)

| Top-level Folder/File | Important Sub-level Folder/File | Purpose                                                                                                                                                  |
|-----------------------|---------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| _includes             |                                 | Contains website "templates"                                                                                                                             |
|                       | `head.html`                     | Template for what the right side of the site webpage (containing the posts) should look like                                                             |
|                       | `sidebar.html`                  | Template for what the sidebar should look like                                                                                                           |
| _layouts              |                                 | Additional "template" files for what the browser window should look like                                                                                 |
|                       | `default.html`                  | Template which creates the default view of the posts (`head.html`) and sidebar (`sidebar.html`) together                                                 |
|                       | `page.html`                     | Template for what a new page (non-post) on the site should look like                                                                                     |
|                       | `post.html`                     | Template for what a post looks like                                                                                                                      |
| _posts                | Many                            | The posts for the website. All posts should follow the specified format:  <br>`---`<br>`layout: post`<br>`title: <TITLE_HERE>`<br>`---`                              |
| donate                |                                 | Logic for the donation page/link.                                                                                                                        |
|                       | `index.html`                    | Template for the donation landing page                                                                                                                   |
|                       | `canceled.html`                 | Template for the view presented when someone cancels out of the donation page                                                                            |
|                       | `success.html`                  | Template for the view presented after a donated has been submitted                                                                                       |
| public                |                                 | Folder which should include any content (e.g. images, documents, etc.) that you wish to display on the site                                              |
| .gitignore            |                                 | Not really applicable when editing just through the GitHub web interface, but ignores certain file types when using the git CLI (command line interface) |
| 404.html              |                                 | Template for page shown when someone tries to access a page that doesn't exist                                                                           |
| README.md             |                                 | File purely used/seen within GitHub, presents an overview of the repository                                                                              |
| _config.yml           |                                 | Within the template files, you can see text surrounded in curly braces `{{ }}`. The values in-between those braces are populated from this file.         |
| about.md              |                                 | Similar to a post in format, changes the content of the "About" page                                                                                     |
| atom.xml              |                                 | Generates the needed XML for someone to add the site to their RSS feed                                                                                   |
| index.html            |                                 | Logic for bringing all the templates together (e.g. next page functionality, display order of posts)                                                     |

## Adding/Editing Content

Main changes that you'll need will probably occur within the `_includes/sidebar.html`, `_posts`, and `about.md` files/folders. All editing/creation of these files/new files can be completed
from the browser. Here's an example of how to edit a pre-existing post:

1. Go to the `_posts` folder

![Click posts](https://i.imgur.com/mfROhpz.png)

2. Click on any post which you'd like to edit, and you'll be presented with a similar view:

![Post_edit_view](https://i.imgur.com/99i4tku.png)

3. Click on the "edit" icon to edit the file and add/change content:

![Edit post](https://i.imgur.com/BxG56go.png)

4. You'll see this view, and can add/edit anything here.

![Change content](https://i.imgur.com/UFMSFaM.png)

5. After you're finished, press the green "Commit changes" button

![Save changes](https://i.imgur.com/bLCrkjV.png)

