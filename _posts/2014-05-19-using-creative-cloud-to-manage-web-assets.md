---
layout: post
title:  "Using the Creative Cloud to Manage Web Assets"
date:   2014-05-18 1:02:32
categories: creative-cloud web
---
In putting this site together I've been trying to dogfood as much as possible. So I did the initial site design in a PSD, used our design comp to code tool to pull out information, and am storing the entire thing in the Creative Cloud. So far it's been a pretty smooth experience. And one thing I've discovered is that the Creative Cloud's file Activity tab is incredibly helpful for managing web assets.

You'll notice this site has a gigantic image as the background. When I initially extracted that asset, it was 1.3 megs. Not ideal for web download. So I took it into Photoshop's save for web, cranked the quality down to zero, and overwrote my inital file. 

Because I was storing it in the Creative Cloud, it kept both copies. I could easily compare the sizes, and I could switch back and forth between them to see the quality. This gave me an idea. Couldn't I test other optimization techniques and compare all of them?

So that's exactly what I did. I pulled out the same image using the Project Parfait web interface, and overwrote my inital file. I also ran the original through [imageoptim](http://imageoptim.com/) to see what impact it had. What was incredibly handy was that I could go to the Creative Cloud web UI and restore the original whenever I wanted to run a new optimization test. 

{:.post-image}
[![Creative Cloud Versions](/img/posts/creative-cloud-versions-thumbnail.png)](/img/posts/creative-cloud-versions.png)

And because file sync would kick in every time I restored a new version, git would pick up the changed file making it easy to commit the changes.

I could see this being *really* helpful for developers who are working with designers that want final say over assets. Most of the developers I've talked to are in charge of doing image optimization on their assets. And in general the tools they use may not result in a loss in quality. But with this workflow, the developer can run whatever optimization tasks they need to, those optimizations are automatically synced to the Creative Cloud, and the designer and go through the revisions to make sure the optimized version looks good. If it doesn't, the designer can simply restore the version they want, leave a comment, and the changed file will sync to the developer's machine. The developer can see the change whenever they do a `git status`. 

You get all the benefit of source control but designers can look at (and control) things visually while the developer can continue to rely on the tools they know. 