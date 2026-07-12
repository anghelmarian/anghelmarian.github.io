# Personal website
Presentation of my personal projects and interests. 

#### Initial setup
```
gem install jekyll bundler
bundle init
bundle
bundle exec
```

#### How to run the website
```
bundle install
bundle exec jekyll build
bundle exec jekyll serve
bundle exec jekyll serve --livereload #to refresh with every change
```

#### Liquid Tips
Liquid = templating language used by jekyll for configuring pages

```
1. Objects = predefined variables used as content for a page "{{ }}", example:
{{ page.title }} #displays page.title variable

2. Tags = define logic and control flow for templates "{% %}", example:
{% if page.show_sidebar %}
    <div class="sidebar">
        sidebar content
    </div>
{% endif %}

3. Filters = change the output of a Liquid obj, separated by "|", example:
{{ "hi" | capitalize }}

```

#### Environments
```
JEKYLL_ENV=production bundle exec jekyll build
JEKYLL_ENV by default is in "development"
```