### CC-05: "The category bar scrolls away on my phone"

> "On smaller screens, the category and filter bar scrolls away instead of
> staying visible at the top while I scroll down through the menu dishes."

Reported by: a student, on a phone
//on laptop sort doesnot work

### CC-09: "The menu shows more dishes than it should"

> "The page is supposed to show a few dishes at a time and load more as
> you scroll. It just dumps a much longer list straight away!"

Reported by: a student

## Notes

- Everything above is reproducible on a fresh clone. If something doesn't
  happen for you, inform us: a complaint that can't be reproduced is itself
  worth reporting
- Some of these need a particular screen size, theme or time of day to
  show up. Part of the task is working out what :)
- Stock can end up in a strange state while you test. Reset it with
  `git checkout -- backend/data/` and restart the server.

## Extra credit

None of this is required, and none of it is needed to clear the task. just brownie points

- **Bugs that are not on this list.** there are problems in this app
  nobody has reported yet: some in what you see on screen, some in what
  the server does. Find one, prove it, and write it up like the rest. Say
  how you noticed it.
- **A test.** Any script or check that fails before your fix and passes
  after.
- **An honest write up** something you spotted but could not fix, or a fix
  you are unsure about, explained clearly. scores better than silence!

Try to keep this in mind: an extra fix should not break anything else! there are **negative points** for this.

Good luck and have fun!
