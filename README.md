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

# floor2

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Round a numeric value to the nearest power of two toward negative infinity.



<section class="usage">

## Usage

```javascript
import floor2 from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-floor2@esm/index.mjs';
```

#### floor2( x )

Rounds a `numeric` value to the nearest power of two toward negative infinity.

```javascript
var v = floor2( -4.2 );
// returns -8.0

v = floor2( -4.5 );
// returns -8.0

v = floor2( -4.6 );
// returns -8.0

v = floor2( 9.99999 );
// returns 8.0

v = floor2( 9.5 );
// returns 8.0

v = floor2( 13.0 );
// returns 8.0

v = floor2( -13.0 );
// returns -16.0

v = floor2( 0.0 );
// returns 0.0

v = floor2( -0.0 );
// returns -0.0

v = floor2( Infinity );
// returns Infinity

v = floor2( -Infinity );
// returns -Infinity

v = floor2( NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import randu from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@esm/index.mjs';
import floor2 from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-floor2@esm/index.mjs';

var x;
var v;
var i;

for ( i = 0; i < 100; i++ ) {
    x = (randu()*100.0) - 50.0;
    v = floor2( x );
    console.log( 'Value: %d. Rounded: %d.', x, v );
}

</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math/base/special/ceil2`][@stdlib/math/base/special/ceil2]</span><span class="delimiter">: </span><span class="description">round a numeric value to the nearest power of two toward positive infinity.</span>
-   <span class="package-name">[`@stdlib/math/base/special/floor`][@stdlib/math/base/special/floor]</span><span class="delimiter">: </span><span class="description">round a double-precision floating-point number toward negative infinity.</span>
-   <span class="package-name">[`@stdlib/math/base/special/floor10`][@stdlib/math/base/special/floor10]</span><span class="delimiter">: </span><span class="description">round a numeric value to the nearest power of 10 toward negative infinity.</span>
-   <span class="package-name">[`@stdlib/math/base/special/round2`][@stdlib/math/base/special/round2]</span><span class="delimiter">: </span><span class="description">round a numeric value to the nearest power of two on a linear scale.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-floor2.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-floor2

[test-image]: https://github.com/stdlib-js/math-base-special-floor2/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-floor2/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-floor2/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-floor2?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-floor2.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-floor2/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-floor2/tree/deno
[umd-url]: https://github.com/stdlib-js/math-base-special-floor2/tree/umd
[esm-url]: https://github.com/stdlib-js/math-base-special-floor2/tree/esm
[branches-url]: https://github.com/stdlib-js/math-base-special-floor2/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-floor2/main/LICENSE

<!-- <related-links> -->

[@stdlib/math/base/special/ceil2]: https://github.com/stdlib-js/math-base-special-ceil2/tree/esm

[@stdlib/math/base/special/floor]: https://github.com/stdlib-js/math-base-special-floor/tree/esm

[@stdlib/math/base/special/floor10]: https://github.com/stdlib-js/math-base-special-floor10/tree/esm

[@stdlib/math/base/special/round2]: https://github.com/stdlib-js/math-base-special-round2/tree/esm

<!-- </related-links> -->

</section>

<!-- /.links -->
