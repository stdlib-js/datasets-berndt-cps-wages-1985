<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# CPS Wages Data

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> A random sample of 534 workers from the Current Population Survey (CPS) from 1985.

<section class="intro">

</section>

<!-- /.intro -->



<section class="usage">

## Usage

To use in Observable,

```javascript
cps = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/datasets-berndt-cps-wages-1985@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var cps = require( 'path/to/vendor/umd/datasets-berndt-cps-wages-1985/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/datasets-berndt-cps-wages-1985@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.cps;
})();
</script>
```

#### cps()

Returns a random sample of 534 workers from the Current Population Survey (CPS) from 1985, including their wages and and other characteristics.

```javascript
var data = cps();
// returns [{...},{...},...]
```

Each `array` element has the following eleven fields:

-   **education**: number of years of education.
-   **south**: indicator variable for southern region (`1` if a person lives in the South; `0` if a person does not live in the South).
-   **gender**: gender of the person.
-   **experience**: number of years of work experience.
-   **union**: indicator variable for union membership (`1` if union member; `0` if not a union member).
-   **wage**: log-transformed wage (in dollars per hour).
-   **age**: age (in years).
-   **race**: ethnicity/race (`'white'`, `'hispanic'`, and `'other'`).
-   **occupation**: occupational category (`'management'`, `'sales'`, `'clerical'`, `'service'`, `'professional'`, and `'other'`).
-   **sector**: sector (`'other'`, `'manufacturing'`, or `'construction'`).
-   **married**: marital status (`0` if unmarried; `1` if married).

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   Based on residual plots, wages were log-transformed to stabilize the variance.

</section>

<!-- /.notes -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/plot@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/datasets-berndt-cps-wages-1985@umd/browser.js"></script>
<script type="text/javascript">
(function () {

var data;
var plot;
var opts;
var x;
var y;
var i;

data = dataset();

// Extract wage data...
x = [];
y = [];
for ( i = 0; i < data.length; i++ ) {
    x.push( data[ i ].age );
    y.push( data[ i ].wage );
}

// Create a plot instance:
opts = {
    'lineStyle': 'none',
    'symbols': 'closed-circle',
    'xLabel': 'Age',
    'yLabel': 'Wage',
    'title': 'Age vs Wage'
};
plot = new Plot( [ x ], [ y ], opts );

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->



<section class="references">

## References

-   Berndt, Ernst R. 1991. _The Practice of Econometrics_. Addison Wesley Longman Publishing Co.

</section>

<!-- /.references -->

<!-- <license> -->

* * *

## License

The data files (databases) are licensed under an [Open Data Commons Public Domain Dedication & License 1.0][pddl-1.0] and their contents are licensed under [Creative Commons Zero v1.0 Universal][cc0]. The software is licensed under [Apache License, Version 2.0][apache-license].

<!-- </license> -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/datasets-berndt-cps-wages-1985.svg
[npm-url]: https://npmjs.org/package/@stdlib/datasets-berndt-cps-wages-1985

[test-image]: https://github.com/stdlib-js/datasets-berndt-cps-wages-1985/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/datasets-berndt-cps-wages-1985/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/datasets-berndt-cps-wages-1985/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/datasets-berndt-cps-wages-1985?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/datasets-berndt-cps-wages-1985.svg
[dependencies-url]: https://david-dm.org/stdlib-js/datasets-berndt-cps-wages-1985/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[cli-section]: https://github.com/stdlib-js/datasets-berndt-cps-wages-1985#cli
[cli-url]: https://github.com/stdlib-js/datasets-berndt-cps-wages-1985/tree/cli
[@stdlib/datasets-berndt-cps-wages-1985]: https://github.com/stdlib-js/datasets-berndt-cps-wages-1985/tree/main

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/datasets-berndt-cps-wages-1985/tree/deno
[umd-url]: https://github.com/stdlib-js/datasets-berndt-cps-wages-1985/tree/umd
[esm-url]: https://github.com/stdlib-js/datasets-berndt-cps-wages-1985/tree/esm
[branches-url]: https://github.com/stdlib-js/datasets-berndt-cps-wages-1985/blob/main/branches.md

[csv]: https://tools.ietf.org/html/rfc4180

[ndjson]: http://specs.frictionlessdata.io/ndjson/

[pddl-1.0]: http://opendatacommons.org/licenses/pddl/1.0/

[cc0]: https://creativecommons.org/publicdomain/zero/1.0

[apache-license]: https://www.apache.org/licenses/LICENSE-2.0

</section>

<!-- /.links -->
