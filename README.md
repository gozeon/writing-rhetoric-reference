# action push gh-pages failed
- https://www.raulmelo.me/en/til/how-to-solve-permission-to-x-denied-to-github-actions-bot

# build

use https://github.com/mhausenblas/mkdocs-deploy-gh-pages
```
# Runs a single command using the runners shell
      - name: Deploy docs
        uses: mhausenblas/mkdocs-deploy-gh-pages@master
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

or

```
- uses: actions/setup-python@v2
        with:
          python-version: 3.x
      - run: pip install mkdocs-material 
      - run: mkdocs gh-deploy --force
```

# reference
- https://github.com/mkdocs/mkdocs
- https://squidfunk.github.io/mkdocs-material/
