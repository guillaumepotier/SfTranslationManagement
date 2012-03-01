# About

little crappy piece of code.
Allow me to find in all my Twig views (with the use of the trans filter that way `{{ "my_key" | trans }}`) and my Php controllers (looking for `->trans('my_key')`) the translations keys used by the solution. Compare them with my `messages.en.yml` file and see what's missing or what have been deprecated

# Use
take this piece of crap and put it into your Symfony's `bin/` directory
give a little 777 chmod rights and then just run `$ .translation_management.sh`


# Output

`Found 312 total translations, 160 found, 152 missing and 39 deprecated`

+ you'll find:

* all translation keys found in /bin/totalmessages.yml
* all missing keys in /bin/missingmessages.yml
* all deprecated keys in /bin/deprecatedmessages.yml