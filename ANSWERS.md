# Answers

## 1. How to run

Open `index.html` in any modern browser.

You can also serve the folder locally:

```bash
npx serve .
```

The app does not need a build step. It does not need React, Vue, npm install, or any other setup.

## 2. Stack and design choices

I used plain HTML, CSS, and JavaScript in one `index.html` file.

I chose this because the app is small. It only needs a form, a weekly grid, buttons, and browser storage. A framework would make the project bigger without adding much value.

For the design, I used a dark background with one bright green accent color. This makes checked days easy to see in the weekly grid.

I also kept the day columns fixed in size. This helps the grid stay readable on both small phones and larger laptop screens.

## 3. Responsive and accessibility

On a small phone screen, the layout becomes tighter. The habit names use the space that is left, and the day buttons become smaller but still easy to tap.

On a larger screen, the app stays centered and the habit name column gets more room.

For accessibility, I made the main controls usable with the keyboard. The check buttons also include labels for screen readers, and the progress bar uses a progress role.

One thing I did not fully handle is the rename field. It works, but it could be better for screen readers. In a bigger version, I would use a normal input or a small dialog for renaming.

## 4. AI usage

I used AI in a limited way while making this project.

It helped me with a few ideas, like how to structure the weekly grid, how to think about the streak counter, and how to keep the layout simple on mobile.

I did not use AI to fully make the project for me. I reviewed the suggestions, changed the parts that did not fit, and made the final choices myself.

For example, the first grid idea was not good enough on small screens, so I changed it. I also adjusted the streak logic so the streak does not reset just because the user has not opened the app yet today.

## 5. Honest gap

The streak counter does not store the date when a habit was created.

Because of that, if someone marks old days after creating a habit, the streak can show history that did not really happen. A better version would save a creation date for each habit and only count streaks after that date.
