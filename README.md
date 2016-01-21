# Rockstar Keyboard Layout Support For The TypeFu App

This is the [rockstar keyboard layout](https://github.com/MadRabbit/rockstar-layout)
support module for the [TypeFu app](http://type-fu.com), which is a really
nice touch-typing training thing.

__NOTE__: this is an unofficial support for the layout. it is totally safe, but
a DIY thing, so be warned.

## How To Install

Type Fu is a hybrid app, it is actually build in javascript and stuff. So, to
install the layout support do the following:

```
cd somewhere/tmp
git clone https://github.com/MadRabbit/typefu-rockstar-support.git
cd /Applications/Type\ Fu.app/Contents/Resources/frontend/
cp somewhere/tmp/typefu-rockstar-support/rockstar.json assets/layouts
edit frontend.js
```

So, basically you need to copy the [rockstar.json](rockstar.json) config into
the `assets/layout` folder in the TypeFu guts. Then open up the `frontend.js`
file and find the `workman` word. You will see an array of supported keyboard
layouts. At the end of the list add `{id: "rockstar", label: "Rockstar"}` to
register the new layout.

After that just restart TypeFu, go into its preferences and you should see the
`Rockstar` option in the list.

Happy training!

## Copyright & License

Dunno, MIT I guess.

Copyright (C) 2016 Nikolay Nemshilov
