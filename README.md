# neotest-vitest

This plugin provides a [Vitest](https://vitest.dev/) adapter for the [Neotest](https://github.com/rcarriga/neotest) framework.

Credits to [neotest-jest](https://github.com/haydenmeade/neotest-jest)

## Known issues
- ~~Wrong error location on collecting results - (this is related to Vitest reporting issue)~~ (solved by Vitest 0.23.0)
- test.each is currently not well supported (currently )

## How to install it
```
use({
  'rcarriga/neotest',
  requires = {
    ...,
    'marilari88/neotest-vitest',
  }
  config = function()
    require('neotest').setup({
      ...,
      adapters = {
        require('neotest-jest') 
        }
    })
  end
})
```

## Usage
![usage preview](https://user-images.githubusercontent.com/32909388/185812063-d05d9cc7-b9aa-43ed-915b-cf156e3f0c52.gif)

See neotest's documentation for more information on how to run tests.

## :gift: Contributing

Please raise a PR if you are interested in adding new functionality or fixing any bugs. When submitting a bug, please include an example spec that can be tested.

To trigger the tests for the adapter, run:

```sh
./scripts/test
```

## Bug Reports

Please file any bug reports and I _might_ take a look if time permits otherwise please submit a PR, this plugin is intended to be by the community for the community.
