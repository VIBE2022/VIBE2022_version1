# Jekyll-Conference-Template

This is a simply academic conference website template, built using Jekyll, using the template github template yishanhe/jekyll-conference-template. To update/edit either edit directly on the github site or to install locally. Updates to this Github site will call Github actions to build the site and will automatically update the github pages site.

To install on your machine, either fork the site (if you intend to pull changes to this site) or clone the site (if you just want a copy for your own use). 
You will need jekyll. Check if jekyll is installed.

```
 jekyll -v
```

If you haven't got jekyll, which is written in Ruby, you will need to install it. Package or collections of Ruby code are called Gems. [Bundler](https://bundler.io) is a package manager for Ruby Gems. Assuming you already have Ruby (which is factory installed on MacOS), the easiest thing is to use  `bundle install` which will read the `Gemfile`, fetch gem metadata from https://rubygems.org/ and install jekyll and other package/dependenices.  `bundle update` will upgrade gems that are already managed by Bundler.  

```
  bundle install
  bundle update jekyll
  jekyll -v
```  
In the top folder, you will find the `Gemfile` and site-specific configurations are in `_config.yml`. If you wish to "serve" the website locally at http://127.0.0.1:4000.

```
  bundle exec jekyll serve
```  

If you are new to Ruby, Gems and Gemfiles, and github pages, the medium posts on [Gem and Gemfiles](https://medium.com/never-hop-on-the-bandwagon/gemfile-and-gemfile-lock-in-ruby-65adc918b856), and [bundler](https://medium.com/@0xcolby/how-does-bundle-install-work-part-1-87a4349c192a) and [github pages](https://www.khanacademy.org/computing/computer-programming/html-css/web-development-tools/a/hosting-your-website-on-github) are useful. 


## Features

- A data file (`_data/conference.yml`) to configure all conference information.
    - `full_title`: conference fullname e.g., First xxx conference on xxxx, 2017.
    - `short_title`: conference shortname e.g., xxxx2017
    - `descriptioin`: short description about the conference (< 160 char)
    - `location`: conference location
    - `logo_path`: conference logo
    - `slideshow`: images slideshow
    - `navbar`: navigation menu.
    - `news`: news section.
    - `sponsors`: sponsor section.
    - `deadlines`: important dates of deadlines, pass-due date will be automatically printed with del line.
    - `social_media`: social media on the navbar. (current support facebook and twitter.)
    - `organizing_committees`: organzizing committees
    - `steering_committees`: steering committees
    - `technical_program_committees`: technical program committees
    - more configuratioins to come.
- Google Analytics: in `_config.yml`
- Font-awesome
- Bootstrap v4.

