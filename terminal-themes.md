# List of Oh-My-Posh themes
Get-ChildItem $env:POSH_THEMES_PATH

## Posh themes path
"C:\Users\Moiz\AppData\Local\Programs\oh-my-posh\themes"
## Custom theme path
"C:\Users\Moiz\.shell-themes"

# Copy themes to customize
Copy-Item "$env:POSH_THEMES_PATH\catppuccin.omp.json" "$HOME\.shell-themes\mycatppuccin.json"

# Customize as needed

# Edit Profile
notepade $PROFILE

## Replace this with new
"oh-my-posh init pwsh --config "$HOME\.shell-themes\mytheme.json" | Invoke-Expression"
