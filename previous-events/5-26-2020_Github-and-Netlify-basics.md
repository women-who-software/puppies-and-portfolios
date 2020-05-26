## Frontend Puppies and Portfolios Series: 
# Getting online quickly with Github and Netlify

**Event Date**: May 26, 2020
<br />
**Event Location**: Online
<br />
**Speaker**: [Jordan Brady](https://twitter.com/mjordancodes)
<br />
**Meetup Page**: [Meetup.com]()

# Part 1: Github

**Github != Git**

![github logo](/images/github-logo.png)

"**GitHub** is a development platform inspired by the way you work. From open source to business, you can host and review code, manage projects, and build software alongside 50 million developers."

![Git Logo](/images/git_hero.png)

"Git is the most widely used modern version control system in the world today. Git is a mature, actively maintained open source project originally developed in 2005 by Linus Torvalds, the famous creator of the Linux operating system kernel. "

*Github provides an interface and platform for working with code that is managed by Git.*

## Create a Github Account:
1. Go to [Github.com](https://github.com)
1. Fill out the form with a username, email address, and password, then press the "Sign up for Github" button.
1. Select the free plan when prompted.
1. Answer the questions about your work and experience.
1. Click the "Complete Setup" button at the bottom of the screen
1. Verify your email address.

## Create a new Repo
1. Click the button to create a new repository.
    - If you just created a github account, you should now be at a screen that asks you "What do you want to do first?" and you should select the option to "Create a repository".
    - If you already had a github account: Click on the green button in the top left area of the main page next to "Repositories" that says "New".
    
    
1. Fill in a name for your new repo, as well as a description (optional, but always helpful). Make sure to keep "Public" selected, and check the box to "Initialize this repository with a README".
    - When everything is all filled out, click the green "Create Repository" button at the bottom of the screen.
1. Next, select the "Create new file" button.
    1. Enter a name for the file of ```index.html```
    1. Copy the content from [here](./index.html) into the new file
    1. Click the "Commit new file" button at the bottom of the screen.


# Part 2: Netlify

![Netlify Logo](/images/netlify-logo-mark.png)

Netlify is a platform for hosting static sites that allows you to publish modern web projects right from your git repos.
There’s nothing to set up & no servers to maintain.

1. Go to: [netlify.com](https://netlify.com)
1. Click the "Sign Up" link in the top right.
1. Select the option to Sign up with Github

Once you have your account created....

1. Select the teal button in the top right to create a "New Site from Git".
1. Under Continuous Deployment, select GitHub
1. This opens up a popup where you should click the green "Authorize Netlify by Netlify" button.
1. Now you can either select "All Repositories" or "Only Selected Repositories". I use only selected.
1. If you picked "Only Selected Repositories" make sure you add your "testing-netlify" repo that we previously created.
1. Click green "Install" Button

You should now be back on the netlify website, still creating a new site.
1. Select the repo you want again, to get to Step 3: Build options and deploy!
1. If you were using a static site generator like gatsby or gridsome, you would need to enter build commands and public details on this screen. Since we have a pure HTML page, we can just hit the go button.

From the Overview screen under Production Deploys, you can watch the progress as your site is published. Since we just have a super basic HTML page for our site, this will be wicked fast.

There will be a link with a random name and numbers at the top. If you click it, it will take you to your live site.

# Part 3: Update Site 

Now that we have connected Netlify to our github repo, all we need to do is make changed in github for the site to be automatically re-deployed.

So if we jump back over to github...

1. Click on the index.html file
1. Select the pencil icon to start editing the page.
1. Add some new text.
1. Click the green "Commit Changes" button at the bottom.

Jump back to Netlify. You may need to refresh the page, but you should now see a second entry under Production Deploys.

# If there is time...

We can also look at:
- Updating name of site to change the Domain
- Set up a Custom Domain
- Using branches to create previews of new code before publishing