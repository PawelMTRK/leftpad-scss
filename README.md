# SCSS Left Pad

Silly implementation of a well-known JS function in SCSS.

## Usage

```scss
@debug leftpad("bar", 5, "_");
// "__bar"

@debug leftpad("foo", 4, "");
// " foo"
```

Used to generate Markdown-like headings:

```scss
@import "leftpad.scss";
// ...

@for $i from 1 through 5 {
    pre:nth-child(#{$i})::before {
        content: leftpad(" ", $i+1, "#");
    }
}
```

## Why?

Cause why not?