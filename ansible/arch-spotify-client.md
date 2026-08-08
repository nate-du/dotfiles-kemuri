Last working version of Spotify Client for Arch with Spicetify - 1.2.79.427

For people using spotify-launcher on archlinux based systems and want to revert to the latest working version of the client, you can follow these steps:

1. Download the deb package linked here: https://discord.com/channels/842219447716151306/842818231706320958/1470736997587881995
2. If your spotify was already updated to the new version that doesn't work, you need to delete it. It should be found at `$HOME/.local/share/spotify-launcher`.
3. From the terminal, run spotify-launcher with these arguments to re-install the client from the deb package you downloaded `spotify-launcher --deb <path_to_deb> --skip-updates`
4. Create a config file for spotify-launcher at `$HOME/.config/spotify-launcher.conf` with the content below to make sure spotify-launcher always starts with the `--skip-update` arguments.
```
[spotify]
extra_arguments = ["--skip-update"]
```