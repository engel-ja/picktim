# Picktim

## Basic JQuery timepicker plugin

## Dependencies
* [JQuery](https://jquery.com) (>=2.2.4)
* [Font-Awesome](https://fontawesome.com) (^4.7)

## Installation

Download the latest release from GitHub at [https://github.com/engel-ja/picktim](https://github.com/engel-ja/picktim).

## Usage

Attach the timepicker plugin to your desired document element, eg.

### HTML

```
<head>
<link rel="stylesheet" type="text/css" href="assets/css/font-awesome/css/font-awesome.css">
<link rel="stylesheet" type="text/css" href="assets/css/picktim/picktim.css">
</head>
<body>
...
<div class="timepicker" id="timepicker"></div>
...
<script type="text/javascript" src="assets/js/jquery/jquery-2.2.4.min.js"></script>
<script type="text/javascript" src="assets/js/picktim/picktim.js"></script>
</body>
```

### Javascript

```
$(".timepicker").picktim();
```

### Options

```
$(".timepicker").picktim({
    backgroundColor: "#EEE",
    borderColor: "#DDD",
    textColor: "#333",
    symbolColor: "#333",
    appendTo: 'body',
    mode: "h24",                 // can be h12 for 12 hour format or h24 for 24 hour format
    orientation: "bottomLeft",   // camel-case combination of (top/bottom and Left/Right) or (left/right and Top/Bottom) 
    defaultValue: '00:00',       // can be set as 'now' to default to current time
    formName: '',                // specifies wether the plugin will be used as part of a form and assigns a name (leave empty for a non-form element)
    icons: {
        up: 'fa fa-chevron-up fa-fw',
        down: 'fa fa-chevron-down fa-fw',
        clear: 'fa fa-times fa-fw'
    }
    });
```

### Useful Method(s)

```
$(".timepicker").picktim('value');  // returns the value of the input element in the plugin
```

## Copyright

Copyright (c) 2018 Adriaan Engelbrecht Licensed under the MIT license.
