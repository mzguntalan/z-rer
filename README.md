# RER

`pip` is simple, amazing, just simply amazing. Rer is wrapper that uses pip, but automatically handles updated the requirements.txt file.

```bash
pip install z-rer
```

`rer` (pronounciation: [ɹɝː]) is useful for simple projects with teams or just solo.

## Demonstration

Use just like `pip`

Instead of `pip install module`, you just do

```bash
rer install module
```

which will automatically update your `requirements.txt` file.

## Recommended Usage

Just like pip can be used with conda for isolated environments, it is recommended to use `rer` together with conda for environment isolation.

## Specific Differences with Pip

Unless stated, `rer` will call `pip` exactly as-is.

1. `install`, `uninstall`: will update the requirements.txt file afterwards.
2. `freeze`: will output `pip list --format=freeze` instead of `pip freeze` which sometimes produces output that can't be `pip`-installed
3. `add`: does the same as `rer install`
4. `init`: creates or overwrites the `requirements.txt` file with the current
