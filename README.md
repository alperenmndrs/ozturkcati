# Öztürk Çatı site preview

Static export of the public-facing WordPress pages for review. It contains rendered HTML and the local assets those pages reference; it does not include WordPress, the database, uploads not used by the pages, or `wp-config.php`.

## Refresh the export

Run this from a machine where the Local site is running at `http://ztrk-at.local`:

```sh
ruby export.rb
```

The GitHub Pages base path in `export.rb` is set to `/ozturkcati`, matching this repository name. After pushing the repository, configure Pages in **Settings → Pages** to deploy from the `main` branch and the root directory.

The contact form depends on WordPress and will not submit from this static preview. Phone and email links remain available.