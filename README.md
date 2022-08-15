# References

https://github.com/purescript/documentation/blob/master/guides/Getting-Started.md

# Install tooling

```
nix-shell -I nixpkgs=https://github.com/NixOS/nixpkgs/archive/00d73d5385b63e868bd11282fb775f6fe4921fb5.tar.gz -p purescript spago nodejs esbuild nodePackages.purescript-language-server
```

# Init a project

```
mkdir my-project
cd my-project
spago init
spago build
spago test
spago run
```

# Run the repl

```
spago repl
```

# Install deps

```
spago install lists foldable-traversable assert
```

# Build for web

```
spago bundle-app
# index.js has been created
```

Now create the index.html.

```
<!DOCTYPE html>
<html>

  <head>
    <meta charset="UTF-8">
    <title>Euler Exercise</title>
  </head>

  <body>
    <script src="./index.js"></script>
  </body>

</html>
```

# Next

Need to read:
- https://book.purescript.org/
- https://github.com/purescript/documentation/blob/master/language/Differences-from-Haskell.md

Check Pursuit for the Purescript 'hackage': https://pursuit.purescript.org/
