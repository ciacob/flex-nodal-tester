# Flex Nodal Tester

A simple test workspace for the [`flex-nodal`](https://github.com/ciacob/flex-nodal) component library.

## Overview

This repository hosts a minimal Apache Flex/AIR application used to exercise the Nodal chart-editing components. It is not intended for production use; the code is purely for demonstrating and stress-testing the library.

## Contents

- `src/nodalworkspace.mxml` – sample application wiring `Nodal` and `SelectionPanel` together.
- `src/nodalworkspace-app.xml` – AIR application descriptor used when launching with `adl`.

## Prerequisites

- [Apache Flex SDK](https://flex.apache.org/) with the AIR runtime.
- A checked out copy of [`flex-nodal`](https://github.com/ciacob/flex-nodal) so its sources or SWC are on your compiler path.

## Building and running

1. Make sure `mxmlc` from the Flex SDK is on your `PATH`.
2. Compile the tester:

   ```sh
   mxmlc -source-path+=path/to/flex-nodal/src -output bin/nodalworkspace.swf src/nodalworkspace.mxml
   ```

3. Launch the AIR application:

   ```sh
   adl src/nodalworkspace-app.xml bin/nodalworkspace.swf
   ```

The UI allows adding and editing sample charts, switching interaction modes and exercising selection handling.

## License

This project mirrors the licensing of `flex-nodal`. See the upstream repository for details.

