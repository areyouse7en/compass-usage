# compass-usage
compass官网的文档描述对使用者来说不够清晰，所以在这一一罗列一下。

对应官网 http://compass-style.org/reference/compass/


```scss
@import "compass/css3";
@import "compass/css3/selection";
.animation {
    @include animation(actionname 1s linear 1s both alternate);
}

@include keyframes(actionname) {
    0% {
        @include transform(translate3D(0, 0, 0));
    }
    100% {
        @include transform(translate3D(50px, 50px, 0));
    }
}

.appearance {
    @include appearance(button);
}

.background-clip {
    @include background-clip(padding-box);
}

.background-origin {
    @include background-origin(padding-box);
}

.background-size {
    @include background-size(50% 50%);
}

.border-radius {
    @include border-radius(50%);
}

.box-shadow {
    @include box-shadow(rgba(blue, 0.4) 0 0 25px, rgba(green, 0.2) 0 0 3px 1px inset);
}

.box-sizing {
    @include box-sizing(border-box);
}

.css-regions {
    @include flow-from(target);
    @include flow-into(target);
}

.column-count {
    @include column-count(4);
    @include column-rule(1px, solid, red);
}

.filter {
    @include filter(hue-rotate(90deg));
}

.flexbox {
    @include display-flex;
    @include flex-wrap(wrap);
    div {
        display: inline-block;
        @include flex(1 0);
        /* non-flexbox browsers */
    }
}

@include font-face("iconfont", font-files("//at.alicdn.com/t/font_1431598591_623468.ttf", "//at.alicdn.com/t/font_1431598591_623468.eot"));
/* font-face */

.hyphenation {
    @include hyphenation;
}

.bg-image {
    @include background-image(linear-gradient(to bottom right, white, #dddddd));
}

.inline-block {
    @include inline-block;
}

.opacity {
    @include opacity(0.5);
}

.selection {
    @include selection(#fe57a1, #fff) {
        font-size: 2em;
    }
    /* @import "compass/css3/selection"; */
}

$default-text-shadow-color: rgba(red, 0.6);
$default-text-shadow-blur: 3px;
$default-text-shadow-v-offset: 1px;
.single-text-shadow {
    @include single-text-shadow;
}

.multi-text-shadow {
    @include text-shadow(rgba(blue, 0.2) 1px 1px 0, rgba(blue, 0.2) 2px 2px 0, rgba(blue, 0.2) 3px 3px 0);
}

.transform {
    @include transform-origin(20%, 30%);
    @include perspective(800);
    @include transform(rotateX(45deg) translateZ(-200px));
}

.transition {
    @include transition(all, 1s, ease, 2s);
}

.user-interface input[type="text"] {
    @include input-placeholder {
        color: #bfbfbf;
        font-style: italic;
    }
}

```
