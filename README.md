# main

This will be deployed as `ghs-athletics.github.io/main`, so the name is up for rework

## getting started

Once `npm` is installed, simply run

```cmd
npm run dev
```

to get started.

## build

```cmd
npm run build
```

Note: Builds are not committed by default.

A github action will automatically build and push to github pages for you (see <https://github.com/ghs-athletics/main/actions> for this process in action)

## file structure

To be honest all frameworks are initially slightly confusing in their file structures,
so here's an incomplete explanation since I also don't completely understand everything:

+ `/pages` holds the actual pages. 
    + `/pages/assets` is not a page
    + `/pages/index` is a page
+ `/public` is similar to `/pages/assets` or something, idk, I will probably consolidate these two folders to make it less confusing
+ `/renderer` is presumably server side rendering (if only static rendering is needed, presumably this will go away. At this early stage it should be easy to switch)
    + `_default.page.server.tsx` is the **root** page
+ `.gitignore`: files ignored automatically when committing
+ `README.md` is what you're reading right now
+ the rest of the files are just configuration, or other metadata that can be ignored, usually

This structure can be compared to the react one: <https://github.com/icecream17/solver/>

