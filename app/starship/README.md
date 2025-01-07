* Windows

Download chocolatey, starship (from chocolatey)

Add file: starship.toml to "D:\config-saving\app\starship\starship.toml" (or your favorite path)

```
$ENV:STARSHIP_CONFIG = "D:\config-saving\app\starship\starship.toml"
Invoke-Expression (&starship init powershell)
```

Then restart your terminal, it should work now

* Ubuntu (Or Linux?)

```
curl -sS https://starship.rs/install.sh | sh
```

say "yes" (it will ask :D)

```
echo '
eval "$(starship init bash)"' >> ~/.bashrc
```

everything should be fine now

Or just go to this [page](starship.rs) and grind again

