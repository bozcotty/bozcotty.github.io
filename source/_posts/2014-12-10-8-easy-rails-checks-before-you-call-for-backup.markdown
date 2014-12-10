---
layout: post
title: "8 Easy Rails Checks Before You Call for Backup"
date: 2014-12-10 14:58:57 -0700
comments: true
categories:
---

New to Rails? New to Code? The following 8 code checks remedy common sequence and syntax-related mistakes you might make when new to Rails, or new to coding in general. Before getting on stack overflow or calling your wizard coding buddy, check these 8 items first.<!-- more -->

1. Did you run
        ```
        $ bundle install
        ```
  after adding those gems to your gemfile?


2. Something not showing up in localhost like you expected? Did your changes change the database in some way? In your terminal window where you're running the local server, hit (ctrl + c), to stop the server, then restart:
  ```
  $ rails s
  ```


3.  Have your run
    ```
    $ rake db:migrate
    ```
 lately? A new migration file does not a full migration make. You need to run this command to get your latest object/model changes into the database. Also, always check the schema file in the db folder to make sure your model tables look right.


4.  Are you in the right directory of your file structure? Check your terminal!


5.  Copy/paste errors. Universal to all programming. Have you checked the easy-to-overlook errors from the last file you copy/pasted from? 'Best to avoid copy/paste if you can and just type everything in.


6.  Are you missing files you swear you've already created and committed to GitHub? You may not be in the same git branch as the one where you made those changes. You could be in the wrong branch, or (see #4 above) in the wrong project directory altogether. Get in the habit of checking your branch whenever you start a new coding session with
  ```
  $ git br
  ```


7.  Syntax errors don't lie. If that's the message you're getting, start looking for typos, missing parens, bad commands and... incorrect syntax.


8.  Did you READ the error message?
Items 1 - 7 when checked, will make your life easier. Item 8? This is the one that's going to make you a much better developer, more quickly. It's natural to fear the error message. Just get over it and start reading them and discovering what they mean. Copy and paste the messages wholesale into a google search and see what comes up. Comprehending error messages will speed up your debugging immensely.

Let me know if you think I've missed some other common mistakes you consistently made when you were new to Rails/coding and maybe I'll amend the list!

