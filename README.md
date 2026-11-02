# Spotter

A phone-first workout planner. Build a plan for any split, watch a 3D demo of every exercise, check your form, see time and calorie estimates, and track your weight, measurements and lifts.

In the gym it gives you a plate calculator with warm-up sets, a note for each exercise, and room to change the workout as you go. A rehab and recovery section, found in the Library and on each exercise's Precautions tab, explains how to train around a sore shoulder, elbow, wrist, back, hip, knee, ankle or neck. It links to the matching structures in [AnatomeX](https://mayank95m.github.io/Anatomex/).

There's no account and no server: the whole app runs in your phone's browser.

Copyright © 2026 Mayank Mayookh. All rights reserved.

## Put it on GitHub Pages

1. On GitHub, create a new public repository, for example `spotter`.
2. Choose **Add file → Upload files** and drag in everything from this folder: `index.html`, `manifest.webmanifest`, `sw.js`, `README.md` and the `icons` folder. Do this from a computer, because phone browsers can't upload folders. Commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, set *Source* to **Deploy from a branch**, pick **main** and **/ (root)**, then save.
4. After a minute or two the app is live at `https://mayank95m.github.io/spotter/` (or whatever you named the repository).

If you use git on the command line instead, run this from inside the folder:

```sh
git init && git add -A && git commit -m "Spotter"
git branch -M main
git remote add origin https://github.com/Mayank95M/spotter.git
git push -u origin main
```

`.nojekyll` is optional. It tells GitHub Pages to serve the files exactly as they are. Your computer may hide it because the name starts with a dot.

## Install it on your phone

- **iPhone:** open the link in Safari, tap Share, then **Add to Home Screen**.
- **Android:** open the link in Chrome, tap the ⋮ menu, then **Install app** (or **Add to Home screen**).

It then opens full screen like an app. After the first visit it also works offline, so a weak signal at the gym won't stop it.

## Your data

- Everything is saved in the browser on your phone. It's tied to the web address you open the app from, so the preview link and your GitHub Pages link each keep their own data.
- To keep a backup, go to **Settings → Export a backup**. To bring it back, use **Restore from a backup**. Use the same steps to move to a new phone or from one link to the other.
- Clearing your browser's site data erases the log. On iPhone, Safari can also remove data for sites you haven't opened in a while. Adding Spotter to the Home Screen and exporting now and then keeps it safe.

## Updating

Replace `index.html` and `sw.js` in the repository with the new versions. Phones pick up the new version the next time the app opens online, usually within a few minutes. Updates never touch your saved data.

## Files

| File | What it does |
|---|---|
| `index.html` | The whole app: code, styles, font and animations in one file. It runs on its own, so you can also drop it into any other static site. |
| `manifest.webmanifest`, `icons/` | Name and icon used when you add the app to your Home Screen. |
| `sw.js` | Keeps a copy of the app on the phone so it opens offline. |
| `.nojekyll` | Optional. Tells GitHub Pages not to process the files. |

## How the numbers are worked out

The full explanation, with references, is in the app under **Settings → How the numbers work**. In short:

- **Calories:** MET value from the 2024 Adult Compendium of Physical Activities × your resting burn (Harris–Benedict, Roza and Shizgal revision) × time spent working and resting. "Active only" mode subtracts what you'd burn sitting still. Expect an error of 20–30%, so treat these as a guide.
- **Time:** sets × reps × the tempo of each animation, plus rest between sets, setup, and a 5-minute warm-up.
- **Weekly sets:** each exercise counts one set for the muscles it trains directly and half a set for the muscles that help. For muscle gain the targets are roughly 8–20 sets per muscle per week, lower for other goals. The plan also points out any muscle you train only once a week.
- **Strength:** estimated 1-rep max uses the Epley formula on sets of 15 reps or fewer. Weight suggestions follow double progression: reach the top of the rep range on every set, then add the smallest practical jump.
- **Body:** body fat uses the U.S. Navy tape method (waist, neck, plus hips for women). The app also shows FFMI, BMI, and maintenance calories (Mifflin–St Jeor × activity).

Spotter gives general training information, not medical advice. If you have an injury or a medical condition, check with a doctor or physiotherapist before starting a new programme.

## Copyright

Spotter is copyright © 2026 Mayank Mayookh. All rights reserved. The Barlow Condensed typeface is by Jeremy Tribby, used under the SIL Open Font License.
