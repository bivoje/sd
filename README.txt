# sd
simple, light, bash scripts for testing or achieving codes

design inspired by git.
produces features make it easy to manage source codes of solvings,
in a number of programming problems.


FEATURES ===============================================================
- you can set default compile command and compile it right away.
- you can test your code working well with specified input-output set


COMMAND LIST (quick reference)
  usage: sd <command> | sd --help

  init | remove                                :before integrity check
    init-initialize, remove-terminate

  set <figname> <val> | get [<figname>..]             :topic configure
    set-set a feature, get show the fig

  co | te | ne                               :with source of a version
    co-compile with options, te-test with IO files
    ne-save current, go to next version

  help | --help                        :when you don't know what to do
    print this manual


MODULES ================================================================
- tester module
provides basic functionality for testing the code including,
interactive compile and testing with given input/output files

- shortc module
provides functionality for version control of the code. each version is
a solution of same problem in different form. as its name denotes,
this functionality is focused on trainig for code golf (short coding)

- sd module
front-end module.
it will import all other module to facilitate the functionallities


NAMING CONVENTIONS =====================================================
names  | denotes functions which
-------|--------------------------
get..    echos value to stdout
set..    set the global variable
[x]_..   returns meaningful value
 x=b      boolean success
 x=v      result value
__..     used for macros
else     user-interaction routines.
auto..   frontend routines.
argn     function - which actually alias -
         checks proper number of argument was given
