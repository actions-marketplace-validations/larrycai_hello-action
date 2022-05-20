![ci workflow](https://github.com/larrycai/hello-action/actions/workflows/hello-action.yaml/badge.svg)

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

Add it as one step to greet

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

## License
The scripts and documentation in this project are released under the [MIT License](LICENSE)
