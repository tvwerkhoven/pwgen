# pwgen
`pwgen` is a command line tool which generates passwords:

    pwgen: OS X password generator
    by Anders Bergh <anders1@gmail.com>

    usage: ./pwgen [options]

    Option:            Meaning:
     -a, --algorithm    Available algorithms: memorable, random
                        letters, alphanumeric, numbers.
                        The default is `memorable'.
     -c, --count        The number of passwords to generate.
     -l, --length       Desired length of the generated passwords.
     -L, --language     Generate passwords in a specified language.
                        Languages: en, de, es, fr, it, nl, pt, jp.
                        Note that this feature is broken and will
                        produce garbage, bug: rdar://14889281
     -h, --help         Prints this message.


## SFPasswordAssistant.h
This project also includes SFPasswordAssistant.h, which is a
reverse-engineered header for Apple's password assistant API
(used in Keychain Access.app, etc).

To use it simply include `SFPasswordAssistant.h` in your project
and link to `SecurityFoundation.framework`.
