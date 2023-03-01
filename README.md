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











<section class="cli">



<section class="installation">

## Installation

To use as a general utility, install the CLI package globally

```bash
npm install -g @stdlib/datasets-berndt-cps-wages-1985-cli
```

</section>

<!-- CLI usage documentation. -->

<section class="usage">

## Usage

```text
Usage: berndt-cps-wages-1985 [options]

Options:

  -h,    --help                Print this message.
  -V,    --version             Print the package version.
         --format fmt          Output format: 'csv' or 'ndjson'.
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   The CLI supports two output formats: comma-separated values ([CSV][csv]) and newline-delimited JSON ([NDJSON][ndjson]). The default output format is [CSV][csv].

</section>

<!-- /.notes -->

<section class="examples">

## Examples

```bash
$ berndt-cps-wages-1985
education,south,gender,experience,union,wage,age,race,occupation,sector,married
8,0,female,21,1,5.1,35,hispanic,other,manufacturing,0
9,0,female,42,1,4.95,57,white,other,manufacturing,0
12,0,male,1,1,6.67,19,white,other,manufacturing,1
12,0,male,4,1,4,22,white,other,other,1
12,0,male,17,1,7.5,35,white,other,other,0
...
```

</section>

<!-- /.examples -->

</section>

<!-- /.cli -->

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

## See Also

-   <span class="package-name">[`@stdlib/datasets-berndt-cps-wages-1985`][@stdlib/datasets-berndt-cps-wages-1985]</span><span class="delimiter">: </span><span class="description">a random sample of 534 workers from the Current Population Survey (CPS) from 1985.</span>


</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

### Community

[![Chat][chat-image]][chat-url]

---

## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/datasets-berndt-cps-wages-1985-cli.svg
[npm-url]: https://npmjs.org/package/@stdlib/datasets-berndt-cps-wages-1985-cli

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
