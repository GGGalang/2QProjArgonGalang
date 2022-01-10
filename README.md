# 2QProjArgonGalang: Latest Update only for AA1.
The repository host for the PASAMA Project, v1.x!

# NOTE: I AM NOW USING THE SITE HOST REPO FOR FUTURE UPDATES. THIS REPO IS DISCONTINUED, AND WILL NO LONGER RECEIVE UPDATES.
By the time you're checking this, the site itself may look a bit different than the zip, there might be new updates, etc. I didn't do this before due to confusion, but please take note of this. Don't worry! The files here are the same as the ones I passed in the original submission in KHUB with the zip (with the exception of this ReadME). The dates might be different due to some github editing stuff but nonetheless, the same.

This project is quite literally the project of a 14-year-old. Please expect imperfections and bugs if you even happen to come across this repo, or if you're my teacher then hi sir!

The PASAMA Project: Paalala SA Mga Madla<br>
Dedicated to serving news and information to the people, from the people. Sources from different yet all reputable outlets and websites, with links for further reading yet a small summary in the form of a paragraph for each news bit. Dedicated to serving true, unbiased information to the best of my ability.

Bugs be expected, easter eggs be found!

## Testing Site:
1. Github Pages: [Here](https://www.pasama.ml/)

##### NOTE: AGAIN, the live site MIGHT BE UPDATED compared to this. This repo is discontinued after all, and I'm already working on AA2.

## READ VERY IMPORTANT (WEBSITE)
As of writing, the site has been up for a fairly long time, but I don't want to take risks on the user's experience. Chrome used to flag the site as dangerous and gives you a pop-up of what I call a "red-alert". I don't think it does it anymore, but just in case it does give you the alert, follow these steps:

#### RED ALERT STEPS
1. Click the "Details" button
2. Click "visit this unsafe site".

Wabam! You're all done, and it should just direct you to the site itself. If the red alert doesn't show up in the first place, great! Nothing to worry about.

### NOTE
As of writing, the red alerts are gone, but you still never know. I'll keep the instructions just in case they come back.

**NOTE:** The Github Pages site will receive updates whenever I commit to github. **As stated, the Github Pages site is recommended for usage, instead of the zip**. Easier access without having to use some storage on your system, and updates are live!

**NOTE:** If you downloaded the release zip onto your system, it won't get updated, unlike the live site on github. You have to manually redownload the releases or directories everytime you want to get news updates (whenever I update, since in the first place this is simply a project) if you want to keep using the system-only version.

============================================================================================================================

## NOTE ON YT EMBEDS:
It's a continuous struggle for website creators to provide a smooth experience for users, and that's the case for this.
YT Embeds do reduce total storage taken when you, dear user, download the repository, but at the cost of the need for wifi
to view the video and an increase in the number of http requests when loading the site.

I considered lazy loading/deferring the requests after seeing solutions online to try and ease the burden on the site,
but the requirement for multimedia files was that they AUTOPLAY. On most if not all lazy loading solutions, they require the user
to click on the video before it actually plays. I haven't actually seen any lazy loading solutions for autoplay vids,
due to the fact that they need to be automatically played.

Maybe I'll keep looking and searching for said solution, but until then, I hope the embeds don't make a difference (except of course
when you aren't connected to the net. Realistically speaking, if this was a website then anyone using it would have net and thus
have the video load.)

=============================================================================================================================

## STYLESHEET NOTES:
1. I didn't bother adding pseudo classes for links such as visited.
It's just weird to see the link be PERMANENTLY a different color, especially if it's a link
like the home/title link or side menu links. I could add a visited state with the same properties but that's simply
impractical.
 - The newsbite links themselves, as well as the home topics a-tags have visited and active states, though.

2. This stylesheet is long so be careful as you might get confused. The classes/ids are generally in order from:
Title Navbar>Side Menu>Main body/Content>Footer>Misc (easter eggs). Ctrl + F always helps!

3. I created more css files for images in each content page so that it won't clutter this one even more.
God knows how long this will be if all image classes are here.

Extra note: All images are sprites, except big ones (like the index banner) where it's impractical to turn them into sprites, and favicon ico files.

============================================================================================================================

## SOME DOCUMENTATION:

## MAIN ARTICLE CODE
##### Here's an example of code for articles, so if you want to add one feel free to copy then paste this.
```
<article>

  <tr>
    <td rowspan="2" class="news-border news-extras">
      <img class="article_pic">
      <br><p class="ten">Credits: CREDITS</p>
    </td>

    <th>
      <h2 class="news-heads"><a href="link">ARTICLE TITLE</a></h2><p>DATE POSTED</p>
    </th>
  </tr>

  <tr>
    <td class="news-border">
      <p style="text-align: left;">ARTICLE MAIN BODYy</p>
    </td>
  </tr>

</article>
```

`<article>`:semantic tag, this does nothing really but it does give others extra information when looking at the code.<br>
`<img class="article_pic">`: replace the class with the image's css class. Or use a direct image. Read EXTRAS below.<br>
Other than that, replace the capitalized things with the appropriate items.<br>
For `CREDITS`, put credit where it's due<br>
for `ARTICLE TITLE` put the article title<br>
for `DATE POSTED` put the date when the article was posted<br>
for `ARTICLE MAIN BODY` just place the paragraph summary of each article (and in-text citation at the end).<br>

Copy paste the result into the last part of the table in the respective topic of your article, right before the `</table>` tag.

### Extras:
-**To add images**, you can create a new spritesheet and create a class for it in the topic's respective css file (each topic has one).<br>
-**You can also just download an image file and directly link that**, but that can lead to optimization issues.<br>
-**If you want to use spritesheets**, I really recommend that you do so only when you create BATCHES of articles, since creating a spritesheet and editing it one-by-one will lead to annoying problems where spritesheet image locations change if you use online spritesheet creators. **You could make your own spritesheet and avoid the problem though**.
>>>>>>> b3c8e195ec9d55da2cab7b2b39a871fd9a9d7d68
