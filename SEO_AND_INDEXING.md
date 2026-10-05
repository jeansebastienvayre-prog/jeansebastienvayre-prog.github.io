# SEO and Google indexing

This version adds:
- a stronger homepage title centered on “Jean-Sébastien Vayre”;
- a unique meta description and keyword list;
- descriptions for the main academic pages;
- WebSite and Person structured data;
- explicit index/follow directives.

Publish from the real Git repository:

git add .
git commit -m "Optimize site for Google indexing"
git push
quarto publish gh-pages

Then in Google Search Console:
1. Add the URL-prefix property: https://jeansebastienvayre-prog.github.io/
2. Submit sitemap.xml.
3. Inspect the homepage URL and request indexing.
4. Optionally request indexing for publications.html and research.html.
