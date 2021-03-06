# space-after-keywords: enforce consistent spacing after keywords

(removed) This rule was **removed** in ESLint v2.0 and replaced by the [keyword-spacing](keyword-spacing.md) rule.

(fixable) The `--fix` option on the [command line](../user-guide/command-line-interface#fix) automatically fixed problems reported by this rule.

Some style guides will require or disallow spaces following the certain keywords.

```js
if (condition) {
    doSomething();
} else {
    doSomethingElse();
}

if(condition) {
    doSomething();
}else{
    doSomethingElse();
}
```

## Rule Details

This rule will enforce consistency of spacing after the keywords `if`, `else`, `for`, `while`, `do`, `switch`, `try`, `catch`, `finally`, and `with`.

This rule takes one argument. If it is `"always"` then the keywords must be followed by at least one space. If `"never"`
then there should be no spaces following. The default is `"always"`.

The following patterns are considered problems:

```js
/*eslint space-after-keywords: "error"*/

if(a) {}

if (a) {} else{}

do{} while (a);
```

```js
/*eslint space-after-keywords: ["error", "never"]*/

if (a) {}
```

The following patterns are not considered problems:

```js
/*eslint space-after-keywords: "error"*/

if (a) {}

if (a) {} else {}
```

```js
/*eslint space-after-keywords: ["error", "never"]*/

if(a) {}
```
