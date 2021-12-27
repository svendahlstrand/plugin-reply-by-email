# ✍️ Reply by email for Micro.blog

Let readers reply to your posts using their default email app.

![](./docs/screenshots.png)

> Your blog posts get a **Reply by email** link. The reader's default email app opens in compose view when they tap that link; your email address and a subject line are already filled in.

## Bells and whistles

* 🛠 Customizable via plug-in settings.
* ✍️ Change the link text to whatever you want. Go bananas! Use emojis!
* ⛳️ Flexible placement in your theme using a Hugo partial.
* 💌 Subject line is automatically set to the blog post title (or post excerpt, if no title is present).
* 🏷 Optionally prefix the subject line with *Reply to* or whatever you want.
* 🎁 Customize the look and feel using CSS.
* 📟 Use the debug console for help with troubleshooting.

## Get started

Hey, fellow microblogger! 👋

This Micro.blog plug-in is still in beta. But it's a working plug-in that you can manually install and play around with. The installation will be a lot easier in the future. So bear with me for now.

To get updates on this project, [follow @sod on Micro.blog](https://micro.blog/sod).

### Install the plug-in

1. Sign in to https://micro.blog in your favorite browser.

2. [Follow this link](https://micro.blog/account/themes/new?plugin=1) or manually go to *Design* → *Edit Custom Themes* and press *New Plug-in*.

3. Enter a fitting *Title* (like Reply by mail).

4. Enter `https://github.com/svendahlstrand/plugin-reply-by-email` inside *Clone URL*.

5. Choose which *Site* you want to install the plug-in.

6. Press *Add Plug-in*

7. Congratulations, the plug-in is installed. On to configuration.

### Configure the plug-in

1. Go to *Plug-ins* and press ⚙️ Settings (for the Reply by email plug-in).

2. Fill your address in *Reply by email*.

3. Make other changes as you see fit.

4. Press *Update Settings* and go to the next step.

### Include the Reply by email link in your custom theme

For this step, you need to set up a custom theme. Maybe you already have one? If not, [follow Manton's instructions here](https://help.micro.blog/t/custom-themes/59).

1. [Follow this link](https://micro.blog/account/themes) or go to *Design* → *Edit Custom Themes*.

2. Click on your custom theme. (It's probably named Marfa Custom or something like that.)

3. Click on the template `layouts/post/single.html`

4. Add this partial call where you see fit: `{{ partial "reply-by-email.html" . }}`. A good place is after the content (look for `{{ .Content }}` in the template).

5. Press *Update Template* and pat yourself on the back.

### Make sure the Reply by email link shows up

1. Find a post on your blog and make sure you see the *Reply by email* link.

2. Click it, make sure it works like expected.

### Having troubles?

If you know how the developer console work in your browser, *Enable debug console* under the plug-in settings. It may help you while troubleshooting.

Feel free to [reach out to @sod on Micro.blog](https://micro.blog/sod) for additional help.
