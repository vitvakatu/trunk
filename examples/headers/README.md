Headers Example
===========
An example demonstrating how to set a custom response headers for Trunk's `serve` command.

Take a look at [`Trunk.toml`](./Trunk.toml) in this directory for an example of how the headers 
can be configured.

This example is based on the usage of [`SharedArrayBuffer`][link] type which is only available 
in the browser if two specific headers are set:
- `Cross-Origin-Opener-Policy: same-origin`
- `Cross-Origin-Embedder-Policy: require-corp`

After opening a page in the browser, go to the browser's dev tools. If you see no error messages 
in the console – everything is working as expected. You can also inspect the response headers in 
the network tab of the dev tools.

[link]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/SharedArrayBuffer
