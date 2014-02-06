## base::shQuote

Escape strings for passing to shell

---

base::**shQuote**(*string*: **Char**, *type*: **Char**)

base::**shQuote**(*string*: **Char**)

> *type* in `c("s", "sh", "cs", "csh", "cm", "cmd")`

If *type* is not supplied, set to `"sh"`.

*Returns* Char.Dim(0) - a character vector of same length as *string*

Each element returned is the string element escaped for passing to a shell of type indicated by *type*

*type* | Shell
-------|--------
"s", "sh" | Bourne Shell, Bash
"cs", "csh" | CShell, TCShell
"cm", "cmd" | Windows Command

---


[R Quote Strings for Use in OS Shells](http://stat.ethz.ch/R-manual/R-patched/library/base/html/shQuote.html)


