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
The simplest way to use these styles is to add the following line to the
**top** of the Intranet site's ``style.css`` file:
```css
@import url("/intranet/styles/css/styles.css");
```

If you do not favour this method of loading additional stylesheets, you may
alternately add the load reference to the ``common/htmlheader.html`` file:
```html
<!doctype html>
<!--[if lt IE 7]><html class="no-js ie ie6 oldie" lang="en"><![endif]-->
<!--[if IE 7]><html class="no-js ie ie7 oldie" lang="en"><![endif]-->
<!--[if IE 8]><html class="no-js ie ie8 oldie" lang="en"><![endif]-->
<!--[if IE 9]><html class="no-js ie ie9 oldie" lang="en"><![endif]-->
<!--[if gt IE 9]><!--><html class="no-js" lang="en"><!--<![endif]-->
<head>
	<title>Claromentis <txt name="title_message"></txt></title>

	<include file="core_head.html">
	<!--- Load special stylesheets -->
	<link rel="stylesheet" type="text/cs" href="/intranet/css/styles.css" />

	<!--- favicon and apple touch icon -->
	<link rel="shortcut icon" href="/images/icons/favicon.ico" type="image/x-icon" />
	<link rel="apple-touch-icon" sizes="57x57" href="/images/icons/intranet-touch-icon-57.png" />
	<link rel="apple-touch-icon" sizes="72x72" href="/images/icons/intranet-touch-icon-72.png" />
	<link rel="apple-touch-icon" sizes="114x114" href="/images/icons/intranet-touch-icon-114.png" />
	<link rel="apple-touch-icon" sizes="144x144" href="/images/icons/intranet-touch-icon-144.png" />
</head>

<body name="body-block">
```

### Bootstrap Extensions
#### Callouts
![](https://raw.githubusercontent.com/LaboratoryGA/styles/master/img/screenshots/callouts.jpg)

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
![](https://raw.githubusercontent.com/LaboratoryGA/styles/master/img/screenshots/panels.jpg)

Coming soon ...

### Fastaction Slider
Coming soon ...

### Grid
Coming soon ...
