# sd
simple, light, bash scripts for testing or achieving codes

design inspired by git.
produces features make it easy to manage source codes of solvings in a number of programming problems.


FEATURES
- you can set default compile command and compile it right away.
- you can test your code working well with specified input-output set


COMMAND LIST (quick reference)
  usage: sd <command> | sd --help

  init | remove                        :before integrity check
    init-initialize, remove-terminate

  set <figname> <val> | get <figname>  :topic configure
    set-set a feature, get show the fig

  co | te                              :with source of a version
    co-compile with options, te-test with IO files

  help | --help                        :when you don't know what to do
    print this manual


MODULES
- tester module
provides basic functionality for testing the code including,
interactive compile and testing with given input/output files

- sd module
front-end module.
it will import all other module to facilitate the functionallities
