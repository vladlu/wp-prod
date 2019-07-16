# About

This is a dev system for WordPress developers which makes life easier. 

# How to use

Just add the rules to `rules` file and run `run.sh` — it will automatically download the
specified version of [wp-prod-core](https://github.com/vladlu/wp-prod-core/) which will parse
and execute the rules.

If you want to uninstall the wp-prod-core, run `uninstall.sh`. It's usually helpfull to free up the disk
space because `node_modules` directory can be large (>50mb & >10k files).

## Other

See a rules sample file here: [wp-prod-core/rules.sample](https://github.com/vladlu/wp-prod-core/blob/master/rules.sample).

See the full list of rules for the specific version of wp-prod-code and nuances of its work on
[its GitHub page]([wp-prod-core](https://github.com/vladlu/wp-prod-core/)).

You can specify the desired version of wp-prod-core in `core-version` file. 
By default, the latest version of wp-prod always contains the latest version of wp-prod-core specified 
(I take care of that). It can be useful only if you want to downgrade the core version.

#

Version: 1.0.3  
Core Version: 1.14.4

License: [MIT](https://github.com/vladlu/wp-prod/blob/master/LICENSE)
