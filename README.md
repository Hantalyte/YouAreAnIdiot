# YouAreAnIdiot

"YouAreAnIdiot" is pure JavaScript code that can mimic the abilities of the original trogan.

## How It Works

The modern implementation of the trogan is difficult for two main reasons: automatic pop-up blockers and strict autoplay policies. While these changes are certainly in the user's favor, they make the original design defunct. However, workarounds are possible.

Google Chrome has various "Chrome URLs," which are various built-in pages accessibile via a "chrome://" scheme. A full list of them can be found by navigated to "chrome://chrome-urls". Obviously, they are unique to Google Chrome and cannot be accessed by another browser.

Chrome URLs are intruiging because, unlike regular websites, the browser's pop-up blockers and autoplay policies no longer apply. Even Chrome Extensions cannot access them. Therefore, if the trogan were to somehow run in one of these pages, it would actually work.

I created JavaScript code that aims to do just that. Once you copy-and-paste it into a Chrome URL's console, found inside DevTools, it behaves just like the original! (or at least, as close as I could get it to be...)

Since it is purely code, the gif and the audio file are embedded into the code as base64 strings. Unfortunately, I was still unable to *directly* replicate the phenomenon whereby it multiplies after you close one window. Instead, the original Chrome URLs by which the code was run serves as a "mastermind" or "puppeteer" of sorts. Whenever the user closes one of its child processes, in addition to a number of other things that predict the user is about to close it, it is the one that creates more minions. It is also the one that makes the windows bounce around the screen and plays the song. So while it appears close to the original, if the user were somehow able to navigate to the mastermind tab and close it, all the children would stop moving, all audio would cease, and procreation would come to a halt. I tried to make this less likely, by immediately putting the user on a different, big tab, and attempting to navigate back while cause children to spawn, it still isn't perfect.

Regardless, I still think it's pretty interesting and it could be used as a fun prank, I guess...

More information can be found by looking at the comments in the JavaScript file.

## Usage

Navigate to either the original JavaScript code file or the minimalist version, and copy it to your clipboard. Next, navigate to any Chrome URL and enter the console inside DevTools. All that's left to do is to paste the code, press enter, and enjoy the ride. :)

Just a forewarning: if left unchecked, this might cause your computer to crash, so make sure to save everything beforehand!
