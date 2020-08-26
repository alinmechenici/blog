---
title: Learning a new language with Audacity and emacs
date: 2017-02-17 14:00:00 +02:00
---

![Learning Swedish using Audacity and 8sidor.se](https://i.imgur.com/38Y3yM9.jpg)

During the COVID-19 lockdown, I decided to do some things I always wanted to do. I think it was the perfect moment to learn the Swedish language (again). 
This time I will try my best to make it fun and so, I am using the technology as much as possible. 

In doing this, for now, I use Audacity with websites like 8sidor.se and other, or any youtube audio in Swedish (including audiobooks and podcasts).

The process it is simple: I just download the audio article from 8sidor.se, or converted it with TTS (text-to-sound), open it with Audacity and select the word with the mouse (or a graphic design pen if you are more fancy) and Ctr+i for split the word and Ctr+b to label it. After a few minutes of mapping the article, just listen it many times, read it loud by following the visual representation of the sound to say it better. You can also record your voice and see if the two graphics looks the same.

I hope this idea helps you do the same with whatever tonal language you choose to learn.

I love emacs. I am using it everyday for a lot of activities like: writing scripts, emails, articles, reading RSS news, PDFs, ePubs, etc. Now I am using it for learning a new language also.
For this, I am using sdcv-mode.el from Elpa. I made the keybinds "C-c s" to translate a word from Swedish to English and Latin at point and "C-c e" to translate from English to Swedish at point. 

![Emacs](/images/screenshot-2020-08-26T131432.png)

(use-package define-word
  :ensure t
  :bind (("C-c e" . define-word-at-point)
         ("C-c E" . define-word)))

(load-file "~/.emacs.d/custom/sdcv-mode.el")
(global-set-key (kbd "C-c s") 'sdcv-search)
(global-set-key (kbd "C-c S") 'sdcv-search-input)


This article will remain a work in progress. So, I will keep you updated here with my learning status, you should do the same in return. :)

