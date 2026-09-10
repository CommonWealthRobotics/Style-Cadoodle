# Style-Cadoodle

CaDoodle's colors, icons, and general look live here. CaDoodle pulls this
repo down at launch and reads whichever theme is active from it, so a theme
merged here reaches every user on their next launch. There is nothing to
build and nothing to publish.

## Themes

Each theme is a single CSS file at the repo root. The file's name is the
theme's name: CaDoodle looks up the active theme by filename, so
`Lavender.css` is what appears as "Lavender" in the theme picker.

The official themes:

- `Bens-PinkerCAD.css`
- `Courtnah.css`
- `Dark-Blue.css`
- `High-Contrast.css`
- `Kala.css`
- `Lavender.css`

User contributed:

- `Milk-Chocolate.css` (aaron4ce)

Open any of them as a working example while you learn the format. They are
the best documentation of what a theme can set, and every one of them is
live in the application today.

## Icons

`light/` and `dark/` hold the application's icons, over 60 in each, one set
per mode. These cover the whole interface rather than only the shape menu:
toolbar actions, view controls, the logo, and the configuration panels.

Each theme's own CSS selects which set it uses, so a light theme and a dark
theme can share everything else and differ only here.

## Contributing a theme

The full walkthrough, including the local edit-and-test loop, is in
[CaDoodle's Theme Customization
docs](https://cadoodlecad.com/tutorial/ThemeCustomization.html). Read that
first if you have not written a theme before.

The short version:

1. Fork this repo.
2. Add your theme as a single `.css` file at the root, named the way you
   want it to appear in the picker.
3. Test it locally, following the docs above, before you open anything.
4. Open a pull request.

Start from a copy of an existing theme rather than an empty file. A theme
that only sets a few properties inherits the rest, and the gaps are easier
to see when you are changing values that already work.
