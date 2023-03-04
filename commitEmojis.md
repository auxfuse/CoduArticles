```bash
git commit -m "initial commit"
```
The commit message here is just so bland....and to be honest, as an example it is very simple in structure and context. But let's say we had scope to add some color and vibrancy to our commit message, something simple, that doesn't require any fancy libraries / installs / compilers.

### Emoji walks on stage 🚶‍♀️🚶‍♂️

```bash
git commit -m "🚀Initial commit"
```
Emojis ✨, such a tiny addition that has now brought some life to this plain text. Did you know that other professions are using Emojis to denote similar context meaning to break through language barriers / dialect differences / and even Accessibility? No, well you do now...and one of the biggest leaders of this adoption is Marketing. Plain and simply put, using Emojis is a method to send a clear, concise, and direct message for categorisation. A single character implementation to express what words in a sentence does. And we can adopt this methodology in our commit messages. I'm not saying we all return to short text world of the early 2000s, but just think about it 😉, in a world where seconds gained can be the difference between just-in-time and out-of-time. ⏰

Want more context? 👀 Peak this [Zendesk Article](https://www.zendesk.com/blog/emojis-for-better-communication/) 👀

And there is a simple and easy way to do this:
* On Windows: Hold `ctrl` on your keyboard and then press `.` (this is a full stop / period symbol).
* On Mac: Hold `ctrl + cmd` and then press `space`.

👆both of these will open your Emoji Picker drawer on your respective OS. If you are using an Android device, just select the Emoji drawer from the touchscreen keyboard.

* Example of Windows Emoji Picker Drawer:
![emojiPicker Screenshot](https://raw.githubusercontent.com/auxfuse/CoduArticles/main/imgs/emojiPicker.PNG)

If that doesn't tickle your fancy, you could always adopt the Common Locale Data Repository (CLDR) Short name:
``` :bug: = 🐛``` or even use Unicode Characters ``` U+1F41B = 🐛 ```. Both of these methods when used, will give you a cute little Bug emoji, which as we all now in Programming...isn't that cute at all. 😭

If you do go down the road of CLDR / Unicode, here is a handy reference guide from the [Unicode.org](https://unicode.org/emoji/charts/full-emoji-list.html) website.

### Historical Usage Edge case & Modern Day:

Now before anyone get's on my case about the purity of a commit and what they should be representing, don't stress. What if I told you that a list of Emojis have been selected for standardisation usage in a commit message? Ayeee, got your attention now right? [Carlos Cuesta and Gitmoji](https://gitmoji.dev/) are available to provide best in content for this. Best of both worlds then, the old guard keeping commit messages pure, and the modern day using Emojis to unilaterally categorise a commit using a single character rather than a word, then followed by the Commit message itself.

Personally, I don't particularly stick to the Gitmoji usage, nor have I installed the CLI Library that comes with it, but I have used it as reference on how to structure commits using standardised Emojis.

Now instead of:
```bash
git commit -m "update: component styles added for carousel"
or
git commit -m "wip: upvote feature for December release"
```

I now type:
```bash
git commit -m "💄: component styles added for carousel"
or
git commit -m "🚧: upvote feature for December release"
```

Go out there and add some flare to your commits! Get funky, creative, and just enjoy the process of it. 🎈😊

What are you thoughts / takes on this? Have you ever used Emojis in commits before?🤔