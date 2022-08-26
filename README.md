# Rust + Typescript Setup

## How this works

- `wasm-pack` compiles rust code to WebAssembly, and generates javascript glue to provide a nice interface
- `npm` is told to use the generated code using local dependecies
- `esbuild` compiles typescript to javacript so it can be run with `node`
- `node` runs the generated javacript, which now knows how to use the WebAssembly

## Why?

- rust is safe, and javascript is javascript
- bLaZINGly FAsT
