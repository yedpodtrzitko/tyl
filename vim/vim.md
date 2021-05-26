# Exit with non-zero return code

Useful in a following scenario:

- your `$EDITOR` is set to `vim`, so it's used during `git` operations.

- you are in middle of `git rebase -i` / `git commit` etc., but you forget to finish something,
so you want to cancel the operation.

One way is to delete everything in the editor and quit via `:q`, which will subequently cancel the operation

The more elegant solution is to use `:cq`, which will exit the editor with
a non-zero return code (ie. error), and this error will cancel the operation.
