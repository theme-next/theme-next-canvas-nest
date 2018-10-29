<h1 align="center"><a href="https://github.com/hustcc/canvas-nest.js">canvas-nest.js</a> for <a href="https://github.com/theme-next">NexT</a></h1>

<h1 align="center">Installation</h1>

<h2 align="center">Step 1 &rarr; Go to NexT dir</h2>

Change dir to **NexT** directory. There must be `layout`, `source`, `languages` and other directories:

```sh
$ cd themes/next
$ ls
bower.json  _config.yml  docs  gulpfile.coffee  languages  layout  LICENSE.md  package.json  README.md  scripts  source  test
```

<h2 align="center">Step 2 &rarr; Get module</h2>

Install module to `source/lib` directory:

```sh
$ git clone https://github.com/theme-next/theme-next-canvas-nest source/lib/canvas-nest
```

<h2 align="center">Step 3 &rarr; Set it up</h2>

Enable module in **NexT** `_config.yml` file:

```yml
canvas_nest:
  enable: true
  onmobile: true # display on mobile or not
  color: '0,0,255' # RGB values, use ',' to separate
  opacity: 0.5 # the opacity of line: 0~1
  zIndex: -1 # z-index property of the background
  count: 99 # the number of lines
```

**And, if you wants to use the CDN, then need to set:**

```yml
vendors:
  ...
  canvas_nest: //cdn.jsdelivr.net/gh/theme-next/theme-next-canvas-nest@1.0.0/canvas-nest.min.js
  canvas_nest_nomobile: //cdn.jsdelivr.net/gh/theme-next/theme-next-canvas-nest@1.0.0/canvas-nest-nomobile.min.js
```

<h1 align="center">Update</h1>

```sh
$ cd themes/next/source/lib/canvas-nest
$ git pull
```
