# ssz-js

Simple Serialize in pure Javascript (SSZ)

FEATURE 2 CHANGE 2

Install:

```bash
$ npm install ssz
```

Install mocha globally:

```bash
$ npm install -g mocha
```

Run tests:

```bash
$ npm test
```

## Usage

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

-   [serialize](#serialize)
    -   [Parameters](#parameters)
-   [deserialize](#deserialize)
    -   [Parameters](#parameters-1)
-   [eq](#eq)
    -   [Parameters](#parameters-2)
-   [deepcopy](#deepcopy)
    -   [Parameters](#parameters-3)

### serialize

[src/index.js:13-109](https://github.com/ChainSafeSystems/ssz-js/blob/769aef6f8c1e1ab5ddae7985b4b90916ac7f22d4/src/index.js#L13-L109 "Source code on GitHub")

Simply Serializes (SSZ)

#### Parameters

-   `value` **([Buffer](https://nodejs.org/api/buffer.html) \| [array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array) \| [number](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number) \| [object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object))** Value to serialize: hash32 (Buffer) | address (Buffer) | int8/16/32 | bytes (Buffer) | array | object
-   `type` **([string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String) \| [object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object))** A type string ('hash32', 'address', 'int8', 'int16', 'int32', 'bytes'), or type array ['hash32'], or type object containing fields property

Returns **[Buffer](https://nodejs.org/api/buffer.html)** the byte output

### deserialize

[src/index.js:118-232](https://github.com/ChainSafeSystems/ssz-js/blob/769aef6f8c1e1ab5ddae7985b4b90916ac7f22d4/src/index.js#L118-L232 "Source code on GitHub")

Simply Deserializes (SSZ)

#### Parameters

-   `data` **[Buffer](https://nodejs.org/api/buffer.html)** bytes (buffer) to deserialize
-   `type` **([string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String) \| [object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object))** A type string ('hash32', 'address', 'int8', 'int16', 'int32', 'bytes'), or type array ['hash32'], or type object containing fields property

Returns **([Buffer](https://nodejs.org/api/buffer.html) \| [array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array) \| [number](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number) \| [object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object))** deserialized value : hash32 (Buffer) | address (Buffer) | int8/16/32/64/256 | uint8/16/32/64/256 | bytes (Buffer) | array | object

### eq

[src/index.js:241-245](https://github.com/ChainSafeSystems/ssz-js/blob/769aef6f8c1e1ab5ddae7985b4b90916ac7f22d4/src/index.js#L241-L245 "Source code on GitHub")

Checks if 2 simply serialized objects are equal (SSZ)

#### Parameters

-   `x` **[Buffer](https://nodejs.org/api/buffer.html)** simply serialized object
-   `y` **[Buffer](https://nodejs.org/api/buffer.html)** simply serialized object

Returns **Bool** the byte output

### deepcopy

[src/index.js:253-256](https://github.com/ChainSafeSystems/ssz-js/blob/769aef6f8c1e1ab5ddae7985b4b90916ac7f22d4/src/index.js#L253-L256 "Source code on GitHub")

Returns a deep copy of a simply serialized object (SSZ)

#### Parameters

-   `x` **[Buffer](https://nodejs.org/api/buffer.html)** Value to deep copy

Returns **[Buffer](https://nodejs.org/api/buffer.html)** the deep copy of x

## Contributors

Very special thank you to [Darren Langley](https://github.com/darrenlangley) for helping build this.
