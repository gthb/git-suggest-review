git-suggest-review
==================

Post-commit hook to nudge you to request a review when modifying files mainly
written by others.

To install, just copy `post-commit` into `.git/hooks` (taking care not to
clobber one that you might have there already).

To handle multiple names for the same committers, put a file `.gitsamenames`
in your home directory containing key value pairs in Python dict literal form
(the hook script places this content inside `{ }`):

    "Joe": "Joe Plumber",
    "joe": "Joe Plumber",
    "joew": "Joe Williams",
