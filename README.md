In our last class you worked on creating web pages and a web site. You started out working locally and then uploaded our code online.

## Local development

You created HTML files locally within a folder called `html`

You downloaded the [Brackets](http://download.brackets.io) editor to edit the files with.

You copied the code you'd written in the first 3 classes into files within the `html` folder.

You viewed the pages in Chrome. This was a big step. You are now doing it all by yourselves!

## Uploading to the web

#### Site44.com (which requires Dropbox)

You signed up via site44.com which sent you to the Dropbox site to accept
It created a folder in how Dropbox/Apps/ folder like:

    /Users/<YOUR_USERNAME>/Dropbox/Apps/site44/<XYZ>.site44.com

XYZ was the name you gave to your site on `Site44.com`

For example I named my site `im-a-muppet` so it created the folder
`/Users/wmernagh/Dropbox/Apps/site44/im-a-muppet.site44.com`

#### Syncing to the internet

My site is online at [im-a-muppet.site44.com](http://im-a-muppet.site44.com).

Any file I place in my folder will be synced with Dropbox and then be available
online.

The contents of the folder are as follows:

```
├── index.html
├── blog
│   ├── about.html
│   ├── best.html
│   ├── mystyle.css
│   └── worst.html
├── images
│   ├── luxembourg.png
│   └── will.png
└── projects
    ├── index.html
    ├── project1.html
    ├── project2.html
    └── project3.html
```

Notice that I have an `index.html` file inside the main folder. This is what
gets displayed by default when you visit [im-a-muppet.site44.com](http://im-a-muppet.site44.com).

Within that file I have links to the projects folder and the blog folder. Both of the folders need to have an `index.html` file also. If they did not you would need to visit [im-a-muppet.site44.com/blog/index.html](http://im-a-muppet.site44.com/blog/index.htm) instead of simply [im-a-muppet.site44.com/blog](http://im-a-muppet.site44.com/blog). Again this is because `index.html` is displayed by default. Without it the server would not know which one to display.

You can see the files [here](https://github.com/impactory/girls_in_tech)

#### Relative links

Ideally you should always use _relative_ paths in your HTML. By this I mean image, style, javascript, and links should not specify https: or http: etc. Instead you should reference the path based on the current location.

In `projects/index.html` I link to project1.html as simply `project1.html` and not `http://im-a-muppet.site44.com/projects/project1.html`

There are a couple of reasons for this:

* The pages will work when you are editing __and__ viewing them locally (i.e. not via the web address). This is handy if you are working without internet access.
* If you have a folder of files (say for a blog or a particular project), moving that folder or renaming the folder will not break the links you have used within the folder.
* If you add a domain name to your site (e.g. im-a-muppet.com) then your links will point to that server and not im-a-muppet.site44.com

#### Domain names

It was hard to cover this because there are many ways this is done and each provider (e.g. site44.com) does it differently. 

If you want to add a custom domain name there are two things that you need.
1. To purchase the domain name.
2. To purchase a plan on site44.com that allows you to use your own domain name.

Starting out it probably makes sense to purchase the domain through site44.com. Getting it associated with you site will be mostly automatic that way.

Alternatively you can purchase the domain with a site like [hover](http://hover.com) and then configure site44.com yourself manually. They have documentation on their site to do this.

The advantage of using hover (or others) are twofold. 1) They may offer more domains; 2) It will be easier to move away from site44.com to an alternative provider if you manage the domain names separately.
