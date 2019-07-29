# About

A production system for WordPress developers which makes life easier. 

# How to use

Just add the rules to the `rules` file and run `run.sh` — it will automatically download the
specified version of [wp-prod-core](https://github.com/vladlu/wp-prod-core/) which will parse
and execute the rules.

If you want to uninstall the *wp-prod-core*, run `uninstall.sh`. It can be helpful if you want
to free up the disk space; because sometimes the `node_modules` directory can be large (usually it is more than 50MB and 10k files).

## Other

- See a rules sample file here: [wp-prod-core/rules.sample](https://github.com/vladlu/wp-prod-core/blob/master/rules.sample).

- See the full list of rules for the specific core version on
[its GitHub page](https://github.com/vladlu/wp-prod-core/).

- You can specify the desired version of the core in `core-version` file. 
By default, the latest version of *wp-prod* always contains the latest version of *wp-prod-core* specified 
(I take care of that). It can be useful only if you are using an outdated version of *wp-prod* or
want to downgrade the *wp-prod-core* version.
   
#
    
* **It has to be installed in the `dev/` directory of the project root to work correctly.**


* It's also recommended to add this to `.gitignore` of your project:

    ```
    # wp-prod
        
    dev/wp-prod/*
    !dev/wp-prod/*.sh
    !dev/wp-prod/rules
    !dev/wp-prod/core-version
    !dev/wp-prod/readme.txt
    ```

#

Version: 1.0.26  
Core Version: 1.14.10

License: [MIT](https://github.com/vladlu/wp-prod/blob/master/LICENSE)
