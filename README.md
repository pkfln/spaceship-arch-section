<h1 align="center">
  📐 + 🚀
  <br>Spaceship Arch Section<br>
</h1>

<h4 align="center">
  Custom spaceship section to display the current CPU architecture (useful for Apple Silicon Macs)
</h4>

<p align="center">
  <a href="https://github.com/pkfln/spaceship-arch-section/releases">
    <img src="https://img.shields.io/github/v/release/pkfln/spaceship-arch-section.svg?style=flat-square"
      alt="GitHub Release" />
  </a>

  <a href="https://github.com/pkfln/spaceship-arch-section/actions">
    <img src="https://img.shields.io/github/workflow/status/pkfln/spaceship-arch-section/ci?style=flat-square"
      alt="GitHub Workflow Status" />
  </a>
</p>

## Installing

You need to source this plugin somewhere in your dotfiles. Here's how to do it with some popular tools:

### [Oh-My-Zsh]

Execute this command to clone this repo into Oh-My-Zsh plugin's folder:

```zsh
git clone https://github.com/pkfln/spaceship-arch-section.git $ZSH_CUSTOM/plugins/spaceship-arch-section
```

Include `spaceship-arch-section` in Oh-My-Zsh plugins list:

```zsh
plugins=($plugins spaceship-arch-section)
```

### [zplug]

```zsh
zplug "pkfln/spaceship-arch-section"
```

### [antigen]

```zsh
antigen bundle "pkfln/spaceship-arch-section"
```

### [antibody]

```zsh
antibody bundle "pkfln/spaceship-arch-section"
```

### [zinit]

```zsh
zinit light "pkfln/spaceship-arch-section"
```

### [zgen]

```zsh
zgen load "pkfln/spaceship-arch-section"
```

### [sheldon]

```toml
[plugins.spaceship-arch-section]
github = "pkfln/spaceship-arch-section"
```

### Manual

If none of the above methods works for you, you can install Spaceship manually.

1. Clone this repo somewhere, for example to `$HOME/.zsh/spaceship-arch-section`.
2. Source this section in your `~/.zshrc`.

### Example

```zsh
mkdir -p "$HOME/.zsh"
git clone --depth=1 https://github.com/pkfln/spaceship-arch-section.git "$HOME/.zsh/spaceship-arch-section"
```

For initializing prompt system add this to your `.zshrc`:

```zsh title=".zshrc"
source "~/.zsh/spaceship-arch-section/spaceship-arch-section.plugin.zsh"
```

## Usage

After installing, add the following line to your `.zshrc` in order to include Arch section in the prompt:

```zsh
spaceship add arch
```

## Options

| Variable                   |              Default               | Meaning                              |
| :------------------------- | :--------------------------------: | ------------------------------------ |
| `SPACESHIP_ARCH_SHOW`   |               `true`               | Show current section                 |
| `SPACESHIP_ARCH_PREFIX` | `$SPACESHIP_PROMPT_DEFAULT_PREFIX` | Prefix before section                |
| `SPACESHIP_ARCH_SUFFIX` | `$SPACESHIP_PROMPT_DEFAULT_SUFFIX` | Suffix after section                 |
| `SPACESHIP_ARCH_SYMBOL` |               `📐·`                | Character to be shown before version |
| `SPACESHIP_ARCH_COLOR`  |             `yellow`               | Color of section                     |

## License

MIT © [pkfln](https://pkfln.io)

<!-- References -->

[Oh-My-Zsh]: https://ohmyz.sh/
[zplug]: https://github.com/zplug/zplug
[antigen]: https://antigen.sharats.me/
[antibody]: https://getantibody.github.io/
[zinit]: https://github.com/zdharma/zinit
[zgen]: https://github.com/tarjoilija/zgen
[sheldon]: https://sheldon.cli.rs/
