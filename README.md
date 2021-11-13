# xkb_fr-BÉPO

## What is "xkb" ?

xkb file is a directory under linux based distribution that rules the keymaps. This means that the logic behind the keys pushed is saved in this directory and so allow us to custom our keyboard layouts.

The path to reach those documents is the following :
```
/user/share/X11/xkb/symbols/
```

## What is the purpose of this repository ?

Here is an archive of my keyboard's layout that allows me to find it wherever I am and also allows community to maybe get inspired by it.

## What's the matter basically ?

It's a custom BÉPO layout improved for coding and fast typing.
BÉPO is basically a French adaptation of the Dvorak layout which has been made for English Dactylography.

The points I touched upon in order to carry out that :

1. Avoiding the dead keys
2. Bringing brackets right under the right hand's fingers
3. Binding slashes on the space bar in order to make navigation easier

|Here is the keymap of my BÉPO version|
|-|
|![image](https://user-images.githubusercontent.com/48366000/141658946-da6947bb-9d0d-490c-b265-a44c4f33ef76.png)|

## What if I want to try it out ?

_Read **entirely** the README if you really want to try it out : probable issues identified at the end_

1. The only way possible is to copy my code and then paste it instead of the previous statement called :

```
default  partial alphanumeric_keys
xkb_symbols "basic" {
```

2. When it's done, make sure you added the correct keyboard layout with `Gnome Settings` or `ibus`.
 - _tips : I advice you to keep your previous layout *INTACT* and just edit another one in case an issue arises._
3. Then you can logout or reboot to refresh the session.
4. Toggle to your new keyboard by selecting it in the 'gui' used by your system or by using the shortcut 'meta + space'

## Boring stuff

 - I'm not responsible of any issue caused while following this tutorial : this is a suggestion of help to use it, that's all (though I struggle to imagine how a problem could occur here…)

There are two worst cases you could face.

The first one is the following :
   - You have only one keyboard layout set up on your system which is not equal to the layout printed on your physical keyboard (or you have a blank keyboard)
   - You _badly_ rewrited the file that rules this layout (making the layout nonfunctional)
   - You logout and you don't succeed to login because the system is using `default QWERTY us`

The second one is :
   - You have only one keyboard layout set up on your system which is not equal to the layout printed on your physical keyboard (or you have a blank keyboard)
   - You _correctly_ rewrited the file that rules this layout BUT you forgot a character that you need for your Session password
   - You logout and you don't succeed to login
