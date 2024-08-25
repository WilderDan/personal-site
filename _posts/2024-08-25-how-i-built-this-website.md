---
layout: post
section-type: post
category: stem
---

You can see the website source code [here](https://github.com/WilderDan/personal-site).

## Why bother?

I wanted to try a new hobby, and making a website seemed fun.
I decided on the blog format because I wanted to improve my writing.
I chose to talk about STEM because I find it interesting - mathematics in particular.
It is also a very broad topic so I should never run out of things to discuss.

I also wanted to use this website to "learn by teaching" (Feynman Technique).
I don't expect or care about getting a large number of people to read my blog.
Making my notes/projects public will encourage myself to improve my writing, teaching, programming, and understanding.
I hope so at least.

I made this for myself, but I hope if you found yourself here that you get something out it.

## Tech Stack

- GitHub: version control, hosting, CI/CD
- Jekyll: Static site generator
- { Personal }: Jekyll Theme found [here](https://github.com/le4ker/personal-jekyll-theme)
- Ruby: To install Jekyll and run locally  

I chose these because I wanted to get a website up and running fast while having a high level of ability to customize.
Also I wanted it to do it for free not counting the custom domain name cost which was optional.

## The Process

### Research

I have done some web development before, but I have not worked with Jekyll or Ruby before.
Perfect time to learn!
I used Jekyll's website for documentation.
Specifically, [this](https://jekyllrb.com/docs/ruby-101/) for the Ruby basics about gems, gemfiles, and bundler, and [this](https://jekyllrb.com/docs/step-by-step/01-setup/) for a step by step tutorial.
Lastly, I searched for responsive minimal theme that just works.
I was already comfortable working with GitHub.

### Installation

1. I forked [{ Personal }](https://github.com/le4ker/personal-jekyll-theme) for my theme.
2. I installed Ruby 3.2.2 with rbenv as a way to pick that specific version (the theme requires it). I use Fedora so I followed [these instructions](https://developer.fedoraproject.org/tech/languages/ruby/ruby-installation.html).
3. `gem install bundler`
4. `bundle install`

### Development

To run locally:

`bundle exec jekyll serve --watch --livereload`

Then visit `localhost:4000` in a browser.

Live reload doesn't work with edits to the _config.yml file.
In that case, I would have to cancel and run again.

The theme authors did a good job. 
The theme looks great on desktop and mobile by default.
It also has icons and a manifest file set up for a web app for your mobile device. 
All set up by default.

I made the following changes after forking the repository.

- Self explanatory edits in the _config.yml file. Namely, content that is not related to theme settings.
- I removed the 'Timeline' and 'Contact' pages.
- I removed Google Analytics, Disqus, and all social buttons except for the one linking to my GitHub page.
- I disabled dynamic typing. 
- I modified js.html to display a random quote specified in _config.yml.
- I made a script for making new posts.

To make a new post (from project root directory):

`./scripts/new-post title-of-my-post-here`

See my [last post]({% post_url 2024-08-23-new-post-script %}) for more details. 


### Deployment

I enabled GitHub Pages on the main branch.
Whenever I push changes, GitHub will build the Jekyll site and deploy automatically.
Nice!

### Custom Domain Name (optional)

I used Namecheap to buy a domain name. 
So far my experience has been positive with them.
Other companies would have worked as well though.

I entered my domain name in GitHub Pages settings and url for project settings in _config.yml.

I created four `A` records on Namecheap
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

I created one `CNAME` record to point `www.wilderdan.com` to `wilderdan.github.io` on Namecheap.

I waited an hour or so and checked enforce HTTPS on GitHub Pages settings.

## Closing Thoughts

I am happy with how the website looks on desktop and mobile.
The 'new post' script and Jekyll's integration with GitHub makes for a nice workflow.
I hope to post new things soon!
