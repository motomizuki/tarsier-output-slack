# tarsier-output-slack

slack input plugin for tarsier.


## install

```bash
pip install tarsier-output-slack
```

## configuration

```yaml
out:
  type: webapi
  webhook_url: https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXX # required
  channel: random # default
  text: | # text that post slack channel
      temperature {temperature}
```

The text can embed `{}` values in the matched field.
see https://docs.python.org/3.6/library/string.html#module-string.
