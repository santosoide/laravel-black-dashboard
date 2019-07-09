# Laravel 5.8 Black Dashboard

This repositories using `laravel-frontend-presets/black-dashboard` from [Creative Tim](https://creative-tim.com/?ref=bdl-readme)

## Clone the repo

```sh
$ git clone git@github.com:cyberid41/laravel-black-dashboard.git
```

## Installation

- `cd laravel-black-dashboard`
- Install dependencies `composer install`
- In your terminal run `composer dump-autoload`
- Run `php artisan migrate --seed` to create basic users table

## Config

### Database
```sh
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=root
```

## Development

```sh
$ php artisan serve
```

## File Structure
```
├───app
│   ├───Http
│   │   ├───Controllers
│   │   │       HomeController.php
│   │   │       PageController.php
│   │   │       ProfileController.php
│   │   │       UserController.php
│   │   │       
│   │   └───Requests
│   │           PasswordRequest.php
│   │           ProfileRequest.php
│   │           UserRequest.php
│   │           
│   └───Rules
│           CurrentPasswordCheckRule.php
│           
├───database
│   └───seeds
│           DatabaseSeeder.php
│           UsersTableSeeder.php
│           
└───resources
    ├───assets
    │   ├───css
    │   │       black-dashboard.css
    │   │       black-dashboard.css.map
    │   │       black-dashboard.min.css
    │   │       nucleo-icons.css
    │   │       theme.css
    │   │       
    │   ├───demo
    │   │       demo.css
    │   │       demo.js
    │   │       
    │   ├───fonts
    │   │       nucleo.eot
    │   │       nucleo.ttf
    │   │       nucleo.woff
    │   │       nucleo.woff2
    │   │       
    │   ├───img
    │   │       anime3.png
    │   │       anime6.png
    │   │       apple-icon.png
    │   │       bg5.jpg
    │   │       card-primary.png
    │   │       default-avatar.png
    │   │       emilyz.jpg
    │   │       favicon.png
    │   │       header.jpg
    │   │       img_3115.jpg
    │   │       james.jpg
    │   │       mike.jpg
    │   │       
    │   ├───js
    │   │   │   black-dashboard.js
    │   │   │   black-dashboard.js.map
    │   │   │   black-dashboard.min.js
    │   │   │   theme.js
    │   │   │   
    │   │   ├───core
    │   │   │       bootstrap.min.js
    │   │   │       jquery.min.js
    │   │   │       popper.min.js
    │   │   │       
    │   │   └───plugins
    │   │           bootstrap-notify.js
    │   │           chartjs.min.js
    │   │           perfect-scrollbar.jquery.min.js
    │   │           
    │   └───scss
    │       │   black-dashboard.scss
    │       │   
    │       └───black-dashboard
    │           ├───bootstrap
    │           │   │   _alert.scss
    │           │   │   _badge.scss
    │           │   │   _breadcrumb.scss
    │           │   │   _button-group.scss
    │           │   │   _buttons.scss
    │           │   │   _card.scss
    │           │   │   _carousel.scss
    │           │   │   _close.scss
    │           │   │   _code.scss
    │           │   │   _custom-forms.scss
    │           │   │   _dropdown.scss
    │           │   │   _forms.scss
    │           │   │   _functions.scss
    │           │   │   _grid.scss
    │           │   │   _images.scss
    │           │   │   _input-group.scss
    │           │   │   _jumbotron.scss
    │           │   │   _list-group.scss
    │           │   │   _media.scss
    │           │   │   _mixins.scss
    │           │   │   _modal.scss
    │           │   │   _nav.scss
    │           │   │   _navbar.scss
    │           │   │   _pagination.scss
    │           │   │   _popover.scss
    │           │   │   _print.scss
    │           │   │   _progress.scss
    │           │   │   _reboot.scss
    │           │   │   _root.scss
    │           │   │   _tables.scss
    │           │   │   _tooltip.scss
    │           │   │   _transitions.scss
    │           │   │   _type.scss
    │           │   │   _utilities.scss
    │           │   │   _variables.scss
    │           │   │   
    │           │   ├───mixins
    │           │   │       _alert.scss
    │           │   │       _background-variant.scss
    │           │   │       _badge.scss
    │           │   │       _border-radius.scss
    │           │   │       _box-shadow.scss
    │           │   │       _breakpoints.scss
    │           │   │       _buttons.scss
    │           │   │       _caret.scss
    │           │   │       _clearfix.scss
    │           │   │       _float.scss
    │           │   │       _forms.scss
    │           │   │       _gradients.scss
    │           │   │       _grid-framework.scss
    │           │   │       _grid.scss
    │           │   │       _hover.scss
    │           │   │       _image.scss
    │           │   │       _list-group.scss
    │           │   │       _lists.scss
    │           │   │       _nav-divider.scss
    │           │   │       _pagination.scss
    │           │   │       _reset-text.scss
    │           │   │       _resize.scss
    │           │   │       _screen-reader.scss
    │           │   │       _size.scss
    │           │   │       _table-row.scss
    │           │   │       _text-emphasis.scss
    │           │   │       _text-hide.scss
    │           │   │       _text-truncate.scss
    │           │   │       _transition.scss
    │           │   │       _visibility.scss
    │           │   │       
    │           │   └───utilities
    │           │           _align.scss
    │           │           _background.scss
    │           │           _borders.scss
    │           │           _clearfix.scss
    │           │           _display.scss
    │           │           _embed.scss
    │           │           _flex.scss
    │           │           _float.scss
    │           │           _position.scss
    │           │           _screenreaders.scss
    │           │           _shadows.scss
    │           │           _sizing.scss
    │           │           _spacing.scss
    │           │           _text.scss
    │           │           _visibility.scss
    │           │           
    │           ├───custom
    │           │   │   _alerts.scss
    │           │   │   _buttons.scss
    │           │   │   _card.scss
    │           │   │   _checkboxes-radio.scss
    │           │   │   _dropdown.scss
    │           │   │   _fixed-plugin.scss
    │           │   │   _footer.scss
    │           │   │   _forms.scss
    │           │   │   _functions.scss
    │           │   │   _images.scss
    │           │   │   _input-group.scss
    │           │   │   _misc.scss
    │           │   │   _mixins.scss
    │           │   │   _modal.scss
    │           │   │   _navbar.scss
    │           │   │   _rtl.scss
    │           │   │   _sidebar-and-main-panel.scss
    │           │   │   _tables.scss
    │           │   │   _type.scss
    │           │   │   _utilities.scss
    │           │   │   _variables.scss
    │           │   │   _white-content.scss
    │           │   │   
    │           │   ├───cards
    │           │   │       _card-chart.scss
    │           │   │       _card-map.scss
    │           │   │       _card-plain.scss
    │           │   │       _card-task.scss
    │           │   │       _card-user.scss
    │           │   │       
    │           │   ├───mixins
    │           │   │       opacity.scss
    │           │   │       _alert.scss
    │           │   │       _background-variant.scss
    │           │   │       _badges.scss
    │           │   │       _buttons.scss
    │           │   │       _dropdown.scss
    │           │   │       _forms.scss
    │           │   │       _icon.scss
    │           │   │       _inputs.scss
    │           │   │       _modals.scss
    │           │   │       _page-header.scss
    │           │   │       _popovers.scss
    │           │   │       _vendor-prefixes.scss
    │           │   │       _wizard.scss
    │           │   │       
    │           │   ├───utilities
    │           │   │       _backgrounds.scss
    │           │   │       _floating.scss
    │           │   │       _helper.scss
    │           │   │       _position.scss
    │           │   │       _shadows.scss
    │           │   │       _sizing.scss
    │           │   │       _spacing.scss
    │           │   │       _text.scss
    │           │   │       _transform.scss
    │           │   │       
    │           │   └───vendor
    │           │           _plugin-animate-bootstrap-notify.scss
    │           │           _plugin-perfect-scrollbar.scss
    │           │           
    │           └───plugins
    │                   _plugin-perfect-scrollbar.scss
    │                   
    └───views
        │   dashboard.blade.php
        │   welcome.blade.php
        │   
        ├───alerts
        │       feedback.blade.php
        │       success.blade.php
        │       
        ├───auth
        │   │   login.blade.php
        │   │   register.blade.php
        │   │   verify.blade.php
        │   │   
        │   └───passwords
        │           email.blade.php
        │           reset.blade.php
        │           
        ├───layouts
        │       │   app.blade.php
        │       │   footer.blade.php
        │       │   
        │       └───navbars
        │           │   navbar.blade.php
        │           │   sidebar.blade.php
        │           │   
        │           └───navs
        │                   auth.blade.php
        │                   guest.blade.php
        │           
        ├───pages
        │       icons.blade.php
        │       language.blade.php
        │       map.blade.php
        │       maps.blade.php
        │       notifications.blade.php
        │       rtl.blade.php
        │       tables.blade.php
        │       table_list.blade.php
        │       typography.blade.php
        │       upgrade.blade.php
        │       
        ├───profile
        │       edit.blade.php
        │       
        └───users
                create.blade.php
                edit.blade.php
                index.blade.php
```