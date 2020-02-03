# Coder Jay's Blog

Use jekyll to generate html & thanks for [Hacker Blog Theme](https://github.com/tocttou/hacker-blog)

## Local Build

1. [`gem install jekyll`](https://jekyllrb.com/docs/installation/#install-with-rubygems)
2. `gem install jekyll-seo-tag`
3. (`cd` to the blog directory, then:) `jekyll serve --watch --port 8000`
4. Go to `http://0.0.0.0:8000/` in your web browser.

*Note: In case have set a `baseurl` different than `/` in `_config.yml`, go to `http://0.0.0.0:8000/BASEURL/` instead.*

### Local build using docker

```bash
docker run --rm -p 8000:8000 \
  --volume="LOCATION_OF_YOUR_JEKYLL_BLOG:/srv/jekyll" \
  -it tocttou/jekyll:3.5 \
  jekyll serve --watch --port 8000
```

Replace `LOCATION_OF_YOUR_JEKYLL_BLOG` with the full path of blog repository. Visit `http://localhost:8000/` to access the blog.

*Note: In case have set a `baseurl` different than `/` in `_config.yml`, go to `http://0.0.0.0:8000/BASEURL/` instead.*

## License

CC0 1.0 Universal
