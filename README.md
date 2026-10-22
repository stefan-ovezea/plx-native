# PR #921 screenshots

Captured from feature commit 71f6e2a2 with the macOS simulator and local mock PMS.
The title, episode names, queue and test-pattern media are synthetic. No household Plex account was used.

- 01: Episode 1, Next focused, Previous disabled before five seconds.
- 02: Episode 2, Previous focused, Next disabled at the end of the queue.
- 03: Right immediately seeks with the HUD hidden while playback continues. Observed: `seek(in-place): av_seek t=12384000000 coalesced=0`.
- 04: Right with the HUD visible moves the pending target; OK has not been pressed and no new seek request was emitted.

The simulator uses its clock sink and simvideo screenshot compositor. These images demonstrate UI states, not LG decoder behavior or TV performance. Captured at 3840x2160 drawable resolution (1920x1080 logical canvas). The layout-only guard-log trigger was armed for capture.
