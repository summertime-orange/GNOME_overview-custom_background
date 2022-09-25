# Custom background for GNOME overview

25 Sep 2022 summertime-orange

Instructions for how to change the overview background in GNOME for a custom shell theme by editing the gnome-shell.css.

## Editing the gnome-shell.css

The gnome-shell.css is located in:
/home/USER/.themes/THEME/gnome-shell/

Replace USER with your username, and THEME with the name of the gnome shell theme you are using.

Open the gnome-shell.css with a text editor and edit the overviewGroup:

#overviewGroup {
  background-image: url("assets/overview_background.png");   /* Path to the custom background image. */
  background-repeat: no-repeat;
  background-size: cover;
}

If this does not work, some later part of the code might have overwritten it. In that case, move the overviewGroup to the end of the gnome-shell.css. This works for GNOME 42, but it should work for other versions too; if not, try similar changes.

