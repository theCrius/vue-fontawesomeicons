vue-fontawesomeicons
=============

I was checking over vue-awesome but I saw lots of "if you have this setup do this" or "if you have this other do that". I wanted a simple component as I did for vue-weathericons that just give me a component-like interface to use font-awesome v4.7 as I don't like the passive aggressive stance of v5.0.

For the moment, there is no support for stacks and lists. I'll work on it or you're welcome to give your contribution.

## Requirements

This package require [font-awesome](https://www.npmjs.com/package/font-awesome) as peer dependency and of course needs to be used inside a VueJS application.

## Installation

``` sh
npm install --save vue-fontawesomeicons
```

## Usage

In your component:

```vue
<script>
import FontawesomeIcon from 'vue-fontawesomeicons';

export default {
  name: 'myComponentName',
  // [...]
  components: {
    FontawesomeIcon
  }
};
</script>

<template>
  <div class="whatever">
    <p>All attributes are optional and non mutually exclusive, apart from the 'icon' of course:</p>
    <fontawesome-icon icon="home" />
    <fontawesome-icon icon="home" spin />
    <fontawesome-icon icon="home" flip="vertical" />
    <fontawesome-icon icon="home" rotate="180" />
    <fontawesome-icon icon="spinner" pulse />
    <fontawesome-icon icon="home" fw pull="left" border />
    <fontawesome-icon icon="home" ariaHidden="false" />
  </div>
</template>
```

## Contributions

All contributions are welcome as they'll help me keep messing up with Vue.
