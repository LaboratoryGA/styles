# Styles
A collection of stylesheets for use with Claromentis 7.x

## Installation
Clone the repository into your Intranet directory structure.
```shell
cd /Claromentis/web
```

### If entire Intranet is under GIT SCM control
Add the repository as a sub-module:
```shell
git submodule add https://github.com/LaboratoryGA/styles.git intranet/styles
```

### If the site is not under GIT SCM control
Make a simple clone of the repository:
```shell
git clone https://github.com/LaboratoryGA/styles.git intranet/styles
```

## Usage
The simplest way to use these styles is to add the following lines to the
**top** of the Intranet site's ``style.css`` file:
```css
@import url("/intranet/css/bootstrap-ext.css");
@import url("/intranet/css/fastaction-slider.css");
@import url("/intranet/css/grid.css");
```

### Bootstrap Extensions
#### Callouts
Although Bootstrap does offer alerts, these are intended as more transient
pieces of visual information. By contrast, callouts provide a similar visual
queue, but are intended more for permanent display in a site, like warnings
or such.

The appearance of these comes from the Bootstrap site itself.

```html
<section class="bs-callout bs-callout-info">
	Something something, dark side ...
</section>
```

#### Panel
Coming soon ...

### Fastaction Slider
Coming soon ...

### Grid
Coming soon ...
