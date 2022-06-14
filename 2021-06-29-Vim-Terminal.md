---
cover: ''
date: 2021-06-29
datetime: 2021-06-29 00:00:00+00:00
description: Vim was made to work with the command line. Many beginners do not understand
  what are the true capabilities of Vim, myself included:) Vim can run terminal comma
edit_link: https://github.com/mr-destructive/techstructive-blog/edit/gh-pages/blog/posts/2021-06-29-Vim-Terminal.md
image_url: https://techstructiveblog.hashnode.dev/_next/image?url=https%3A%2F%2Fcdn.hashnode.com%2Fres%2Fhashnode%2Fimage%2Fupload%2Fv1624873886869%2FjUY_IzcWe.png%3Fw%3D1600%26h%3D840%26fit%3Dcrop%26crop%3Dentropy%26auto%3Dcompress%2Cformat%26format%3Dwebp&w=1920&q=75
long_description: Vim was made to work with the command line. Many beginners do not
  understand what are the true capabilities of Vim, myself included:) Vim can run
  terminal commands without leaving the text editor, open an instance of a terminal,
  work with shell envir
now: 2022-06-14 05:54:44.185681
path: blog/posts/2021-06-29-Vim-Terminal.md
slug: vim-plus-teminal
status: published
subtitle: To feel and live in Vim with the terminal.
tags:
- vim
- linux
templateKey: blog-post
title: 'Vim: Terminal Integration'
today: 2022-06-14
---

## Vim and Terminal!?
Vim was made to work with the command line. Many beginners do not understand what are the true capabilities of Vim, myself included:) Vim can run terminal commands without leaving the text editor, open an instance of a terminal, work with shell environments, and other things depending on the use case.

## Running Terminal/ shell commands from within Vim

You can run the commands from inside of Vim by just using `:!` before the command, this means you have to be in command mode. Just after being in command mode, the ! or bang operator will execute the command typed after it from the terminal(Linux/ macOS) or your default shell(Windows -> CMD/Powershell).
```
:!pwd
```
The above command from vim will redirect to the terminal and show the output of the command and return on pressing any key. In this case, it will execute the PWD command and just wait for the user to enter any key to return to Vim.

The following is an example of how it could be used from Vim in Windows using Powershell as the default shell.

![Animation.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1624885870237/Ie5C-3u1B.gif)

In Windows, dir is equivalent of ls for Linux. That was not the best example of how a terminal can be used at its best, You can also use a logical operator from within vim to run multiple commands at once. 

### Running programs/ code from Vim on terminal

This becomes quite a great feature for making Vim from a text editor to an IDE, this can be paired with Keymaps i.e when the user types certain keys, the command gets executed making the code run from the terminal. I have already used this feature to set up Vim for python, bash, and other programming languages. Also, I have written an article about  [keymapping](https://dev.to/mrdestructive/vim-keymapping-guide-3olb)  and Vim setup for  [Python](https://dev.to/mrdestructive/setting-up-vim-for-python-ej)  and  [Bash](https://techstructiveblog.hashnode.dev/vim-setup-for-bash-scripting), this will give you an idea of how to setup vim for any programming language. 

Vim can really shine in this kind of feature as it just becomes flawless and a smooth experience even for a beginner. We just have to run the compile the code and run its executable/ output file, rather for python and other interpreted languages, we have to just pass the file name to the interpreter and that's it.  

## Opening instance of Terminal within Vim.

Vim can also create an instance of the terminal within its window by making a split. This is quite similar to VS Code and other Text editors that have the functionality to create an instance of the terminal within itself. This feature is useful for developing complex systems and depending on the use case, it can be quite important and efficient as well. 

The terminal can be created in various ways the most preferred way is by typing in `:term` from Vim. 
This will create a horizontal split from the current editor and split it into half. You can change the size of the split using the mouse according to your preference. 

![vimtermsplit.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1624888468392/wR0JT8SBN.gif)

Here Vim has certain variables and shortcuts to make things even simpler, say you want to parse the current file to the terminal for execution. You can surely type the name manually or you can be a bit smarter and use % instead, the `%` symbol will parse the file name along with the extension in the terminal. Also `%:r` will parse filename without the extensions(.txt/.py/etc) to the terminal.

There are many things you can do with terminals surely, but with Vim that even goes further than the limits. Terminal/command line is quite important in any development environment as it is an interface for the user to interact with the Operating System. Vim is quite powerful and behaves as a gecko for programmers because it changes itself according to our needs flawlessly and **efficiently**.


![vimpython.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1624891655340/5f81Dpp_O.gif)

Integrating Terminal into a Text Editor truly lights up the environment for development. It becomes an easy and enjoyable experience to test out the code without wasting much time on the actual execution process. Surely it needs time to set up the environment to speed things, for that understanding of the programming and development environment is required. Happy Viming :)
<div class='prevnext'>
    <style type='text/css'>
    :root {
      --prevnext-color-text: #eefbfe;
      --prevnext-color-angle: #ff6600;
      --prevnext-subtitle-brightness: 3;
    }
    [data-theme="light"] {
      --prevnext-color-text: #1f2022;
      --prevnext-color-angle: #ffeb00;
      --prevnext-subtitle-brightness: 3;
    }
    [data-theme="dark"] {
      --prevnext-color-text: #eefbfe;
      --prevnext-color-angle: #ff6600;
      --prevnext-subtitle-brightness: 3;
    }
    .prevnext {
      display: flex;
      flex-direction: row;
      justify-content: space-around;
      align-items: flex-start;
    }
    .prevnext a {
      display: flex;
      align-items: center;
      width: 100%;
      text-decoration: none;
    }
    a.next {
      justify-content: flex-end;
    }
    .prevnext a:hover {
      background: #00000006;
    }
    .prevnext-subtitle {
      color: var(--prevnext-color-text);
      filter: brightness(var(--prevnext-subtitle-brightness));
      font-size: .8rem;
    }
    .prevnext-title {
      color: var(--prevnext-color-text);
      font-size: 1rem;
    }
    .prevnext-text {
      max-width: 30vw;
    }
    </style>
    
    <a class='prev' href='/technical-writer-journey'>
    
        <svg width="50px" height="50px" viewbox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M13.5 8.25L9.75 12L13.5 15.75" stroke="var(--prevnext-color-angle)" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"> </path>
        </svg>
        <div class='prevnext-text'>
            <p class='prevnext-subtitle'>prev</p>
            <p class='prevnext-title'>My Journey as a Technical Writer</p>
        </div>
    </a>
    
    <a class='next' href='/techstructive-blog-init'>
    
        <div class='prevnext-text'>
            <p class='prevnext-subtitle'>next</p>
            <p class='prevnext-title'>What's in Techstructive Blog</p>
        </div>
        <svg width="50px" height="50px" viewbox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M10.5 15.75L14.25 12L10.5 8.25" stroke="var(--prevnext-color-angle)" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
        </svg>
    </a>
  </div>