# Ultimate Water System

AAA-quality, fully fledged water simulation plugin for Unity, with such functionalities as dynamic water physics, buoyancy, foam, wet lens and many more!

## Info

* current version: 2.0.0
* current hot-fix: b1
* [documentation](https://docs.google.com/document/d/1pHTvNq1u5rpVR4wS_QD5bjGNtdL8pY0q7f9BGGAmXX4/edit)

## Issues

The template below should be used as a start for your Issues.
It contains Unity and UWS version, hardware specs and your Unity profile name,
so we are able to contact you through Unity forum. 

```
Description of the problem.
Steps attempted to solve it.

**unity:** 2017.2.0f3
**uws version:** 1.0.0 
**spec:** Intel Core i7, Geforce 640M, Intel HD 4000, ... 
**issued by:** [@your_forum_name](_link to UWS forum post if it exists_)
```

## Hot-fixes 
Hot-fixes contain all the issues currently solved (before they enter offical asset store updates).
Note that it's not a stable release, so be careful.
You can access the newest hot-fix through: [hotfix-page](http://goo.gl/nBx7dS)

Step-by-step guide:
- input the _invoice/order number_ and press _download newest hotfix_
- with the project open in Unity, double-click on the downloaded package, 
and import-replace all the files.

## FAQ

Q: I'm using Playway Water in my project and want to add Ultimate Water System, how?

A: You should first delete all files assotiated with the PW package. The UWS codebase is not backwards compatible with PW and trying to merge them will cause huge headache. 


## Troubleshooting

#### After upgrading from PW asset to Ultimate Water System, _Texture has out of range width / height_ error occurs.
The _Water Quality Settings_ can become corrupted when upgrading, try deleting it. The problem is discussed in [Issue #12](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/12)
