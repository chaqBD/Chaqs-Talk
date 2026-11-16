# Chaqs' Talk

Shakir's doctoral research journal — notable findings from the supply chain
literature, and case studies of AI applied to real supply chain problems.
Built as a static Jekyll site and published with GitHub Pages.

## Adding a new post

1. Create a new file in `_posts/` named `YYYY-MM-DD-short-title.md`.
2. Start it with front matter, e.g.:

   ```yaml
   ---
   title: "Your Post Title"
   categories: ["Literature Review"]   # or ["Case Study"]
   tags: [demand-forecasting, machine-learning]
   excerpt: "One or two sentences shown on the homepage."
   ---
   ```

3. Write the body in Markdown. Two useful custom blocks:
   - A "Key takeaways" list: end a bullet list with `{: .key-points}` on its
     own line right after it, to render it as a highlighted callout box.
   - A pull quote: end a `>` blockquote with `{: .pull-quote}` to render it
     as a large italic quote.
4. Commit and push to `main` — GitHub Pages rebuilds the site automatically.
   There is no build step to run yourself.

Two example posts in `_posts/` show both formats (Literature Review and Case
Study) — delete or replace them once you have real content, they're clearly
marked as placeholders.

## Local preview (optional)

Requires Ruby + Bundler.

```sh
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000/Chaqs-Talk/`.

## Site settings

Title, tagline, and description live in `_config.yml`. Visual design lives in
`assets/css/style.scss`.
