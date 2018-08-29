# Laravel Nova Tab

Custom Nova field to render tabs


![Edit](http://take.ms/MFDjX)
![Detail](http://take.ms/44q7f)
![Validation](http://take.ms/S6hZI)

## Installation

Install the package into a Laravel app that uses [Nova](https://nova.laravel.com) with Composer:

```bash
composer require arsenaltech/nova-tab
```

## Usage

Extend App\Nova\Resource from Arsenaltech\NovaTab\Resource

```php
use Arsenaltech\NovaTab\Resource as TabResource;

abstract class Resource extends TabResource
```

Add the field to your resource in the `fields` method:

```php
use Arsenaltech\NovaTab\NovaTab;

new NovaTab('Address Information', $this->addressFields()),
new NovaTab('Other Information', $this->otherFields()),

```

