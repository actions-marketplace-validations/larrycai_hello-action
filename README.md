![ci workflow](https://github.com/larrycai/hello-action/actions/workflows/hello-action.yml/badge.svg)

# hello-action

Hello world github action

## What's new

Nothing is new, just Hello world, enjoy Github Actions

## Usage

### Inputs

* `who-to-greet`: The name of the person to greet. Default `"World"`.

### Outputs

### `time`

The time we greeted you.

## Example usage

Since add it as one step to greet

```yaml
    steps:
    - name: Hello action step
      id: hello
      uses: larrycai/hello-action@main
      with:
        who-to-greet: 'Larry Cai'
    # Use the output from the `hello` step
    - name: Get the output time
      run: |
        echo "The time was ${{ steps.hello.outputs.time }}"
```

## Implementation examples

* [larrycai/hello-action](https://github.com/larrycai/hello-action), self testing
* [larrycai/hello-pythin](https://github.com/larrycai/hello-python), combile with other actions

## Contributing
We would love for you to contribute to `larrycai/hello-action`, pull requests are welcome! Please see the [CONTRIBUTING.md](CONTRIBUTING.md) for more information.

## License
The scripts and documentation in this project are released under the [MIT License](LICENSE)