Sublime Text PageLines Snippets
==================

This is a [Sublime Text][sublime] package which includes a bunch of handy snippets for develop for [PageLines DMS][pagelines] by [Enrique Chavez][enriquechavez].

## Installation ##

### With Package Control ###

* Bring up the Command Palette (Command+Shift+P on OS X, Control+Shift+P on Linux/Windows).
* Select Package Control: Install Package.
* Select __PageLines Snippets__ to install.
* That's it.

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

__opt_check__

```php
// CheckBox
${1:\$options}[] = array(
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'check',
    'title'     => __('${3:title}','${4:domain}')
);
```

__opt_color__

```php
// Color Picker
${1:\$options}[] = array(
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'color',
    'title'     => __('${3:title}','${4:domain}'),
    'default'   => '#${5:FFFFFF}' // Always set a default value
);
```

__opt_count__

```php
// Count Select
${1:\$options}[] = array(
    'key'          => \$this->id.'_${2:key_name}',
    'type'         => 'count_select',
    'title'        => __('${3:title}','${4:domain}'),
    'count_start'  => ${5:1},   // Starting Count Number
    'count_number' => ${6:10},  // Ending Count Number
    ${7:'suffix'       => '%'  // * Added to the end of the value and optional}
);
```

__opt_check__

```php
// Icon Selector
${1:\$options}[] = array(
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'select_icon',
    'title'     => __('${3:title}','${4:domain}')
);
```

__opt_image__


```php
// Image Upload
${1:\$options}[] = array(
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'image_upload',
    'title'     => __('${3:title}','${4:domain}'),
    'imgsize'   => '${5:16}',         // * The image preview 'max' size
    'sizelimit' => '${6:512000}',     // * Image upload max size default 512kb
);
```

__opt_link__


```php
// Link
${1:\$options}[] = array(
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'link',
    'title'     => __('${3:title}','${4:domain}'),
    'url'       => '${5:http://google.com}',
    'classes'   => '${6:btn-info}'  // You can also use btn-primary, btn-warning, btn-success, btn-inverse
);
```

__opt_menu__


```php
// Select Menu
${1:\$options}[] = array(
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'select_menu',
    'title'     => __('${3:title}','${4:domain}')
);
```

__opt_multi__


```php
// Multi Select
${1:\$options}[] = array(
    'type'      => 'multi', // Here you can nest multiple options
    'title'     => __('${2:title}','${3:domain}'),
    'opts'      => array(
        array(
            ${4://Inner options}
        ),
        array(){
            // Another Option
        }
    )
);
```

__opt_template__


```php
// Template
${1:\$options}[] = array(
    'span'      => 2
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'template',
    'title'     => __('${3:title}','${4:domain}'),
    'template'  => ${5:\$template}
);
```

__opt_text__


```php
// Text Field
${1:\$options}[] = array(
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'text',
    'title'     => __('${3:title}','${4:domain}')
);
```

__opt_textarea__


```php
// TextArea Field
${1:\$options}[] = array(
    'key'       => \$this->id.'_${2:key_name}',
    'type'      => 'textarea',
    'title'     => __('${3:title}','${4:domain}')
);
```

[sublime]: http://www.sublimetext.com/
[sublime3]: http://www.sublimetext.com/3
[pagelines]: http://pagelines.com
[enriquechavez]: http://enriquechavez.com
[package_control]: http://wbond.net/sublime_packages/package_control

