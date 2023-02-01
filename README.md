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

# isNumericArray

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is a numeric array.



<section class="usage">

## Usage

```javascript
import isNumericArray from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-numeric-array@deno/mod.js';
```

#### isNumericArray( value )

Tests if a value is a numeric array.

```javascript
import Int8Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-int8@deno/mod.js';

var bool = isNumericArray( new Int8Array( 10 ) );
// returns true

bool = isNumericArray( [ 1, 2, 3 ] );
// returns true

bool = isNumericArray( [ '1', '2', '3' ] );
// returns false
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: update once Buffer wrapper -->

<!-- eslint no-undef: "error" -->

<!-- eslint-disable no-buffer-constructor -->

```javascript
import Buffer from 'https://cdn.jsdelivr.net/gh/stdlib-js/buffer-ctor@deno/mod.js';
import Int8Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-int8@deno/mod.js';
import Uint8Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-uint8@deno/mod.js';
import Uint8ClampedArray from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-uint8c@deno/mod.js';
import Int16Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-int16@deno/mod.js';
import Uint16Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-uint16@deno/mod.js';
import Int32Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-int32@deno/mod.js';
import Uint32Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-uint32@deno/mod.js';
import Float32Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-float32@deno/mod.js';
import Float64Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-float64@deno/mod.js';
import isNumericArray from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-numeric-array@deno/mod.js';

var arr = new Int8Array( 10 );
var bool = isNumericArray( arr );
// returns true

arr = new Uint8Array( 10 );
bool = isNumericArray( arr );
// returns true

arr = new Uint8ClampedArray( 10 );
bool = isNumericArray( arr );
// returns true

arr = new Int16Array( 10 );
bool = isNumericArray( arr );
// returns true

arr = new Uint16Array( 10 );
bool = isNumericArray( arr );
// returns true

arr = new Int32Array( 10 );
bool = isNumericArray( arr );
// returns true

arr = new Uint32Array( 10 );
bool = isNumericArray( arr );
// returns true

arr = new Float32Array( 10 );
bool = isNumericArray( arr );
// returns true

arr = new Float64Array( 10 );
bool = isNumericArray( arr );
// returns true

arr = [ 1, 2, 3 ];
bool = isNumericArray( arr );
// returns true

bool = isNumericArray( [] );
// returns false

bool = isNumericArray( {} );
// returns false

bool = isNumericArray( null );
// returns false

bool = isNumericArray( new Buffer( 10 ) );
// returns false
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/assert/is-array`][@stdlib/assert/is-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array.</span>
-   <span class="package-name">[`@stdlib/assert/is-number-array`][@stdlib/assert/is-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object of numbers.</span>
-   <span class="package-name">[`@stdlib/assert/is-typed-array`][@stdlib/assert/is-typed-array]</span><span class="delimiter">: </span><span class="description">test if a value is a typed array.</span>

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

[npm-image]: http://img.shields.io/npm/v/@stdlib/assert-is-numeric-array.svg
[npm-url]: https://npmjs.org/package/@stdlib/assert-is-numeric-array

[test-image]: https://github.com/stdlib-js/assert-is-numeric-array/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/assert-is-numeric-array/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/assert-is-numeric-array/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/assert-is-numeric-array?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/assert-is-numeric-array.svg
[dependencies-url]: https://david-dm.org/stdlib-js/assert-is-numeric-array/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/assert-is-numeric-array/tree/deno
[umd-url]: https://github.com/stdlib-js/assert-is-numeric-array/tree/umd
[esm-url]: https://github.com/stdlib-js/assert-is-numeric-array/tree/esm
[branches-url]: https://github.com/stdlib-js/assert-is-numeric-array/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/assert-is-numeric-array/main/LICENSE

<!-- <related-links> -->

[@stdlib/assert/is-array]: https://github.com/stdlib-js/assert-is-array/tree/deno

[@stdlib/assert/is-number-array]: https://github.com/stdlib-js/assert-is-number-array/tree/deno

[@stdlib/assert/is-typed-array]: https://github.com/stdlib-js/assert-is-typed-array/tree/deno

<!-- </related-links> -->

</section>

<!-- /.links -->
