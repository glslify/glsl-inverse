# glsl-transpose
Transpose a matrix in GLSL.

# Example

```glsl
#pragma glslify: transpose = require(glsl-transpose)

void main() {
  mat3 m = mat3(1, 2, 3,
                4, 5, 6,
                7, 8, 9);

  mat3 mt = transpose(m);

  //now mt is the transpose of m
}
```

# Usage

Install with npm:

```
npm install glsl-transpose
```

Then use with [glslify](https://github.com/stackgl/glslify).

# API

```glsl
#pragma glslify: transpose = require(glsl-transpose)
```

### `mt = transpose(float|mat2|mat3|mat4 m)`
Computes the transpose of a matrix

* `m` is a matrix to transpose, either `float, mat2, mat3` or `mat4`

**Returns** The transpose of `m`

# License
(c) 2014 Mikola Lysenko. MIT License