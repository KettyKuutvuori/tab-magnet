# Tab Magnet

An interaction prototype for browser tabs that behave like magnets.

People keep dozens of tabs open across several windows. Regrouping them takes many small clicks and long, precise drags, one tab at a time, so most people give up and the mess stays. Tab Magnet explores a different approach: bring a tab or window close to another and it is pulled in; let go and they snap together. Tabs that belong to the same task attract more strongly, so related work finds its way back together with less effort.

## What you can try

| Behavior | How |
| --- | --- |
| Merge windows | Drag a window by its handle toward another window. In the pull range it is drawn in; in the snap zone the incoming tabs preview in the target strip. Release to merge. |
| Bring similar | Hold <kbd>Shift</kbd> while dragging a tab. Tabs from the same task leave their windows and follow. |
| Tab menu | Right-click (or long-press) a tab to gather its group into its window, move the group to a new window, or close duplicates. |
| Sort all | The magnet button in each tab strip sorts every window by task, type or site. Undo reverts. |
| Duplicates | The magnet menu folds duplicate tabs into their first copy. |
| Move freely | Hold <kbd>Alt</kbd> while dragging a window to move it without snapping. |

The page also has a playlist that demonstrates each behavior automatically with a scripted cursor. It plays once when the demo first comes into view; choose **Play all** or pick a single behavior to watch it again.

## What it explores

- Whether nearness can replace exact drop targets.
- Whether one gesture can move a whole group (Shift-drag collecting scattered tabs).
- What a browser should count as "similar": the same task, the same type of page, or the same site.

In this demo each tab's task is set by hand. A real browser would infer it from where a tab was opened, what the page is about and how the person has grouped tabs before.

## Related work

Vivaldi tab stacks and the tab groups in Firefox and Chrome group tabs by dropping one onto another, through menus, or with AI suggestions. Haiku OS snaps window tabs together by proximity. Tab Magnet adds merging whole windows by nearness and gathering scattered similar tabs in a single drag.

## Running it

It is a single self-contained file. Open `index.html` in a browser, or serve the folder with any static host (for example GitHub Pages). The only external resources are the Geist and Geist Mono fonts from Google Fonts.

The prototype respects the system "reduce motion" setting: animations are skipped and the playlist does not start by itself.

## Status

Interactive prototype. Next step: a comparison test against ordinary drag and drop.
