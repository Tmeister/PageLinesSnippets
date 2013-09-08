Sublime Text PageLines Snippets
==================

This is a [Sublime Text][sublime] http://some.com package which includes a bunch of handy snippets for develop for [PageLines DMS][pagelines] by [Enrique Chavez][enriquechavez].

## Installation ##

### Without Package Control ###

This package is not yet in [wbond's][package_control] repository, so you gotta use Terminal and git to install it.

I'm using [Sublime 3][sublime3] and it works like a charm.

#### Mac OS ####

    cd "~/Library/Application Support/Sublime Text 3/Packages"

#### Windows 7 ####

    cd "C:\Users\YOUR_USERNAME\AppData\Roaming\Sublime Text 3\Packages"

#### Inside _Packages_ ####

    git clone https://github.com/Tmeister/PageLinesSnippets.git "PageLinesSnippets"

### Manually

* Download the .zip file from the GitHub downloads modal
* Unzip the files and rename the folder to "PageLinesSnippets"
* Copy the folder to (~/Library/Application Support/Sublime Text 3/Packages) or (C:\Users\YOUR_USERNAME\AppData\Roaming\Sublime Text 3\Packages)
* Sublime 2 copy the folder to your Sublime Text 2 user packagers directory (`~/Library/Application Support/Sublime Text 2/Packages/User/)

## Available Snippets ##

__opt_button__

```php
${1:\$options}[] = array(
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'select_button',
    'title'     => __('${3:title}','${4:domain}'),
);
```

[sublime]: http://www.sublimetext.com/
[sublime3]: http://www.sublimetext.com/3
[pagelines]: http://pagelines.com
[enriquechavez]: http://enriquechavez.com
[package_control]: http://wbond.net/sublime_packages/package_control

