# Theme NexT Canvas Nest

![Theme Version](https://img.shields.io/badge/NexT-v7.3.0+-blue?style=flat-square)

[canvas-nest.js](https://github.com/hustcc/canvas-nest.js) for [NexT](https://github.com/theme-next).

## Install

### Step 1 &rarr; Go to Hexo dir

Change dir to **Hexo** directory. There must be `scaffolds`, `source`, `themes` and other directories:

```sh
$ cd hexo
$ ls
scaffolds  source  themes  _config.yml  package.json
```

### Step 2 &rarr; Create `footer.swig`

Create a file named `footer.swig` in `hexo/source/_data` directory (create `_data` directory if it does not exist).

Edit this file and add the following content:

```xml
<script color="0,0,255" opacity="0.5" zIndex="-1" count="99" src="https://cdn.jsdelivr.net/npm/canvas-nest.js@1/dist/canvas-nest.js"></script>
```

You can customize these options.

### Step 3 &rarr; Set it up

In the NexT `_config.yml`, uncomment `footer` under the `custom_file_path` section.

```yml
# Define custom file paths.
# Create your custom files in site directory `source/_data` and uncomment needed files below.
custom_file_path:
  #head: source/_data/head.swig
  #header: source/_data/header.swig
  #sidebar: source/_data/sidebar.swig
  #postMeta: source/_data/post-meta.swig
  #postBodyEnd: source/_data/post-body-end.swig
  footer: source/_data/footer.swig
  #bodyEnd: source/_data/body-end.swig
  #variable: source/_data/variables.styl
  #mixin: source/_data/mixins.styl
  #style: source/_data/styles.styl
```
