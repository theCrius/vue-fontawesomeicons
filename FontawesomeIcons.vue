<template>
  <i class="fa" :class="[
    icon ? 'fa-' + icon : '',
    size ? 'fa-' + size : '',
    flip ? 'fa-flip-' + flip : '',
    pull ? 'fa-pull-' + pull : '',
    rotate ? 'fa-rotate-' + rotate : '',
    border ? 'fa-border' : '',
    spin ? 'fa-spin' : '',
    pulse ? 'fa-pulse' : '',
    fixed ? 'fa-fw' : ''
  ]"
  :aria-hidden="ariaHidden"></i>
</template>

<script>
import "node_modules/font-awesome/scss/font-awesome.scss";

export default {
  props: {
    icon: { required: true, type: String },
    size: String,
    flip: String,
    pull: String,
    rotate: Number,
    border: Boolean,
    spin: Boolean,
    pulse: Boolean,
    fixed: Boolean,
    ariaHidden: Boolean = true
  }
}
</script>
