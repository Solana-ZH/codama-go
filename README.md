# Copyma

_Solana Go Client Generator, Powered by Codama_

This package provides a Solana Go client renderer for [Codama](https://github.com/codama-idl/codama)  that generates Go client code from Solana program IDL files.

This tool is in beta, so please report any issues or feedback.

## Installation

```sh
pnpm install cogoma
```



## Usage

Once you have a Codama IDL, you can use the `renderVisitor` of this package to generate go clients. You will need to provide the base directory where the generated files will be saved and an optional set of options to customize the output.

```ts
// node ./codama.mjs
import { renderVisitor } from 'cogoma';

const pathToGeneratedFolder = path.join(__dirname, 'clients', 'go', 'src', 'generated');
const options = {}; // See below.
codama.accept(renderVisitor(pathToGeneratedFolder, options));
```
