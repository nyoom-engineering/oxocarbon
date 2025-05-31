# Contributing

## What is a port?

A port is an adaptation of Oxocarbon's palette for an application of tool. Along with setting colors, it shuold also handle themeing of UI components where necessary to align more with Nyoom Engineering's design ideals.

## Creation

Ports are expected to be MIT liscensed and should follow the naming scheme of `oxocarbon-*` e.g. for alacritty, `oxocarbon-alacritty`. Exceptions can be made for schemes that *must* use a different liscense (e.g. KDE themes should use GPL liscensing).

Make sure to read through the [style guide](https://github.com/nyoom-engineering/oxocarbon/blob/main/docs/style-guide.md) before attempting a port.

You can create ports using [this](https://github.com/nyoom-engineering/oxocarbon-template) public template as a blueprint. It's recommended to follow the instructions below instead of using github's "Use this template" feature, as that leaves a small `generated from <template>` message.

1. Create a repo and leave it empty

```bash
mkdir oxocarbon-name_of_your_port
cd oxocarbon-name_of_your_port
git init
```

2. Add this template as a remote:

```bash
git remote add template https://github.com/nyoom-engineering/oxocarbon-template.git
```

3. Pull from it

```bash
git pull template main
```

4. Delete the remote

```bash
git remote remove template
```

5. Make the new repo its own repository

```bash
git reset $(git commit-tree HEAD^{tree} -m "feat: initial commit")
```

6. Set up the rest of your port, and push it to your user repository!

## Repo Notes

Although you just created the repo successfully, it's important to style it properly to ensure consistency:

- The name of the repo must be the simplest, all lowercase version of the app's name (e.g `nvim` instead of `NeoVim`). You may use hyphens if needed (e.g. `windows-files`).
- Any images should **not** be uploaded to the respository. Instead, its recommended to drag-and-drop the image into a blank github issue and use the generated link instead. This helps keep the repository & clone as small as possible.
- Format the repo's description as "A port of Oxocarbon to <app name>", where <app name> is the name of the app, capitalized properly.
Add oxocarbon to the topics.
- Ensure uppercase meta files (e.g. README.md)
- Don't add health files (e.g. CODE_OF_CONDUCTS.md, SUPPORT.md), those are organization-wide files managed by the organization

## Submission

Ports should first be created under your own profile. Once you feel a port is ready for review, create a PR to this repository with the following

1. A brief description of the application you're porting to
2. A link to the repo with the port
3. A link of your port added to the `README.md` under the `Ports` section

Its also recommended (but not required) to share the port with our discord community beforehand, so that other members of the community can give their opinion on it. It might not be perfect the first time and thats okay! You can choose to keep your port unofficial, or submit a PR and we can work on moving it to the `nyoom-engineering` github organization.