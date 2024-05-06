## This is my console website!
This is very much still a work in progress, but I think it is important to keep it deployed throughout my work on it. It is hosted [here](https://www.alex-werner.com).
## Things I would like to fix
* Currently there are two copies of `index.html`, one in the main directory and one in the `wordstreak` directory. All other `index.html` files are soft links to the one in `wordstreak`. This is because they need file paths to the scripts, which depends on the URL. Because GitHub is hosting this page (and it is then sent over to my website), I have not looked into how to dynamically load the `index.html` file so that I don't need two copies. (The reason they're in separate folders is so that people can go to the links such as `/wordstreak/` directly instead of having to go through the command tree)
* I would like to abstract away more of the console logic. Currently things such as creating lists of options is manually done, with a callback function for when they're created so that I can register the options with what I would like to to with them. Further to this point, I'd like to organize my files better so that all of the console helper functions are in `console.js`. Currently, some are in `main.js`, which is the main shell script.
