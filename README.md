# Vivid Violet

## Prerequisite

Check if **configuration.yaml** allows themes loading from themes folder:

```yaml
frontend:
  themes: !include_dir_merge_named themes
```

And if the **themes** folder exists in **config** folder.

Create when none exist.

### Manual installation

1. Copy `vivid_violet.yaml` to the themes folder
2. If you want the background image, copy `vivid_violet.jpg` to `www\backgrounds`
3. If you want the font, copy the `proxima-nova-font` folder to `www\`
4. Restart Home Assistant

### Enable the Background

1. In your lovelace, click on `Configure UI > Raw configuration editor`
2. Add the code below at the very beginning of the page

```yaml
background: var(--background-image)
```

### Enable the font

1. Go to `Configuration > Lovelace Dashboards > Resources`
2. Add the following to resources and select the **Resource Type:** stylesheet

```html
/local/proxima-nova-font/ProximaNova-Regular.css
```

### Enable the theme

- Open your **Profile** in Home Assistant and select the theme called **Vivid Violet**
