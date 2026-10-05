# Google indexing preparation

This version renders only the public `.qmd` pages.

Technical Markdown files such as:
- LINK_AUDIT.md
- PUBLISH_GITHUB.md
- README_FIRST.md
- INDEXING_GOOGLE.md

are not rendered as public HTML pages and should therefore not appear in the generated sitemap.

After replacing your local project files with this version:

1. `git add .`
2. `git commit -m "Prepare site for Google indexing"`
3. `git push`
4. `quarto publish gh-pages`

Then submit:
https://jeansebastienvayre-prog.github.io/sitemap.xml

in Google Search Console.
