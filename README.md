# How to install themes:
### Step 1:
Download one of the theme files (ex. `Hatsune_Miku.min.css`).

Find where Steam is installed to.
> *(For regular users it should be: `C:\Program Files (x86)\Steam\`)*

Navigate to the `steamui\css` folder.
> *(For regular users it should be: `C:\Program Files (x86)\Steam\steamui\css`)*

Move the downloaded theme file into the `css` folder.

Your files should look something like this:
![image](https://github.com/user-attachments/assets/84995c35-7e3d-4f57-a6d6-1c2b7e0dad92)

---

### Step 2:
Open Steam with the Developer Console enabled.
> For those who don't know what this means, check [here](https://steamcommunity.com/sharedfiles/filedetails/?id=873543244).

Open DevTools with Ctrl+Shift+I or F12. Focus the window that says `DevTools - Steam`.
> You can close the `DevTools - SharedJSContext` window.

Go to the **Console** tab in DevTools.

![image](https://github.com/user-attachments/assets/fb05a676-f14e-41b4-8eff-844df1e4fcd5)


Paste this code in!
> It may ask you to type `allow pasting` before things can be pasted.

Before you press enter, remember to change the file name based on your theme!

This includes the `.min.css` portion of the filename.

```js
let theme_file_name = 'Hatsune_Miku.min.css'
    
ns=document.createElement('link');ns.href='/css/'+theme_file_name;ns.rel='stylesheet';document.head.appendChild(ns);
```

Press enter to submit the command, and viola!

Your theme should now be working.

![image](https://github.com/user-attachments/assets/c5116f92-d7de-423d-9653-8f2d5de80bec)

Keep in mind this is not automated, you will have to do this everytime Steam restarts.

I will work on a theme selector + more. Check back for updates!
