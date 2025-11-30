# Writing Guidelines (wip)

## Cloning and Pushing Repo
The Blowfish theme that our website uses is added as a submodule. To run the Hugo server locally it is important that this is also pulled when the repo is cloned. The `--recurse-submodules` is needed when the repo is cloned.

```
git clone --recurse-submodules https://github.com/TechHutTV/techhut.tv.git
```
Pushing and committing changes can be done with the following.
```
git add -A
git commit -m "what I did"
git push
```

## Images and Video
Make sure images have a descriptive file name with the number prefix being the order they appear in the article. All images **must** be .jpg, .jpeg, or .png with a strong preference of .jpg.
```
├── cover.jpg
├── images
│   ├── 1_zen-browser.png
│   ├── 2_zed-code-editor.png
│   ├── 3_tabby-terminal.png
│   ├── 4_cider-apple-music.png
│   └── 5_betterbird-email.jpg
└── index.md
```

Locally hosted videos can be added just like images in .mp4 or .webm format. File sizes must be under 50mb. See example below for HTML tagging of video.
```
{{< video src="images/cloning_panels_cc.webm" controls="yes" >}}
```
Youtube videos use the default hugo shortcodes.
```
{{< youtube y_8wcMBJrVo >}}
```


## Structure and URL
Folder name should match what we want the url to be ie. linus-rust-drama-cosmic-alpha. Also, going forward we
will exclude the url template tag so that news article fall under a date scheme in the url bar.
