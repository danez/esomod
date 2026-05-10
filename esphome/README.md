For the esphome to work you need to create several helpers:

`sensor.esomod_last_seen` is provided by ESPHome directly.

### esomod_last_watered:

Template:

```
{{ state_attr('input_datetime.esomod_last_watered', 'timestamp') | as_datetime() }}
```

DeviceClass: Timestamp
