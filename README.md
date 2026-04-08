# SandyEmpowers.com

Jekyll site for `sandyempowers.com`.

## Local Development

### Ruby version

This repo includes a [.ruby-version](.ruby-version) file.

If you use `rbenv`, entering the repo should usually select that Ruby version automatically. If it does not, check that `rbenv` is initialized in your shell and confirm the active version with:

```sh
ruby -v
rbenv version
```

To see which Ruby versions you already have installed:

```sh
rbenv versions
```

If the version from [.ruby-version](.ruby-version) is not installed yet, install it and re-enter the repo:

```sh
rbenv install "$(cat .ruby-version)"
```

If you do not use `rbenv`, make sure your shell is already using a compatible Ruby before running Bundler.

### Install dependencies

Install the gems from [Gemfile](Gemfile) / [Gemfile.lock](Gemfile.lock):

```sh
bundle install
```

### Helper scripts

Run the local dev server with live reload:

```sh
./scripts/serve
# bundle exec jekyll serve --livereload
```

Then open:

```text
http://127.0.0.1:4000
```

One-off site build:

```sh
./scripts/build
# bundle exec jekyll build
```

Clean generated output:

```sh
./scripts/clean
# bundle exec jekyll clean
```
