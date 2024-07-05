# AutoPlayPause
A small code to play/pause YouTube videos on switching tabs.

# How To?
1. Open Chrome.
2. Then open YouTube or other video streaming platform.
3. Open `Developer Tools` by shortcut `CTRL + SHIFT + I`.
4. Open Console Tab.
5. Clear by shortcut `CTRL + L`.
6. Copy and Paste the code below in it :
```
document.addEventListener('visibilitychange', () => {
  const video = document.querySelector('video');
  if (document.hidden) {
    video.pause();
  } else {
    video.play();
  }
});
```
7. Press Enter.
8. Close the developer tools.
9. Now, when switch to new tab or open new tab then the video is paused and when returned to youtube video it plays automatically.
