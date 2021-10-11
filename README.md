# Setup

1. Install Emacs:

```
git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d
```

1. Symlink spacemacs configuration from this repo:

```
ln ~/myemacs/spacemacs.el ~/.spacemacs
```

1. Install language server:

```
npm install -g pyright
```

1. Set up github forge using [these instructions](https://magit.vc/manual/ghub/Getting-Started.html#Getting-Started)

1. MacOS Only: Install [flycut](https://apps.apple.com/us/app/flycut-clipboard-manager/id442160987?mt=12)

1. Install dependencies with 

```
pip install -r requirements.txt
npm install -g package.json
```

1. For Rust support: Install `rust-analyzer`
