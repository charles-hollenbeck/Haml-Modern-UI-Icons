# Haml Partials for the [Modern UI Icons][Modern UI Icons]

I made this repo due to wanting an easy way to load in the icons from [Modern UI Icons][Modern UI Icons] and be able to recolor them. All of the files in this repo were made with a quick ruby script I cooked up in about a 5 minute time period so please make an issue or pull request if any of the icons are broken/incorrect/throw an error.

The github repo from where I pull all the original icons/files can be found [here][WindowsIcons].

## Features
* Easy load in
* Can color the icons easily

## Usage
To use an icon from the pack load it into your Haml normally, just make sure to include the local for color otherwise it'll throw an error. An incorrect color will not be the end of the world, it'll just be a black icon.

```ruby
= haml :"icons/<icon name>", :locals => {:color => "#F00"}
```

** Example: **
```ruby
= haml :"icons/appbar.acorn", :locals => {:color => "#F00"}
```

[Modern UI Icons]: http://modernuiicons.com/
[WindowsIcons]: https://github.com/Templarian/WindowsIcons