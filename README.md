# Bourbon-Family
Sass boilerplate starring Bourbon, Neat &amp; Bitters, mixed up with some Normalize.css - ready to be served!

## Installation
Simply download this repository and put everything inside the `src` folder where your `*.scss` files go - all partials are imported through `main.scss`.
For testing / updating, have a look at `package.json`:
- `npm start`: Does nothing, this repo is really just for copy & paste.
- `npm run setup`: Installs npm packages & ruby gems for testing purposes.
- `npm run test`: Creates two versions of `main.css` (ruby-sass + node-sass), making sure everything's working.
- `npm run update`: Runs a (very) basic update script (use with caution).

## Why?
It's just a simple starter including bourbon + family (by [thoughtbot](https://thoughtbot.com/)) and Normalize.css (by [Nicolas Gallagher](http://nicolasgallagher.com/)):
- Bourbon v5.0.0.beta.7 ([Github](https://github.com/thoughtbot/bourbon), [Website](http://bourbon.io))
- Neat v2.0.0 ([Github](https://github.com/thoughtbot/neat), [Website](http://neat.bourbon.io/))
- Bitters v1.5.0 ([Github](https://github.com/thoughtbot/bitters), [Website](http://bitters.bourbon.io/))
- Normalize.css v7.0.0 ([Github](https://github.com/necolas/normalize.css), [Website](http://necolas.github.io/normalize.css/))
- .. also looking forward to Empties/Refills, but right now they are not compatible with Neat v2

Normally after installing Bourbon, Neat & Bitters, you'd get this ..

```
├── base
│   ├── _base.scss
│   ├── _buttons.scss
│   ├── _forms.scss
│   ├── _layout.scss
│   ├── _lists.scss
│   ├── _media.scss
│   ├── _tables.scss
│   ├── _typography.scss
│   └── _variables.scss
├── bourbon
│   ├── bourbon
│   └── _bourbon.scss
└── neat
    ├── neat
    └── _neat.scss
```

.. but since most of my projects are organized the [SMACSS](https://smacss.com) way, I wanted a simple drop-in solution. Sparing the need to install Normalize.css every time, I just included it, accompanied by custom resets (inspired by [inuitcss](https://github.com/inuitcss)):

```
├── base
│   ├── _buttons.scss
│   ├── _forms.scss
│   ├── _layout.scss
│   ├── _lists.scss
│   ├── _media.scss
│   ├── _tables.scss
│   └── _typography.scss
├── utility
│   ├── _box-sizing.scss
│   ├── _normalize.scss
│   ├── _reset.scss
│   └── _variables.scss
├── vendor
|   ├── bourbon
|   │   ├── bourbon
|   │   └── _bourbon.scss
|   └── neat
|       ├── neat
|       └── _neat.scss
└── main.scss
```

## Special Thanks
I'd like to thank everybody that's making free & open source software - you people are awesome. Also I'm always thankful for feedback and bug reports :-)
