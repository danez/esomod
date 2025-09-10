For the esphome to work you need to create several helpers:


### esomod_last_seen:

Template:
```
{% if states.sensor.esomod_battery_voltage.last_updated > states.sensor.esomod_sleep_mode.last_updated %}
{{ states.sensor.esomod_battery_voltage.last_updated }}
{% else %}
{{ states.sensor.esomod_sleep_mode.last_updated }}
{% endif %}
```

DeviceClass: Timestamp

### esomod_last_watered:

Template:

```
{{ state_attr('input_datetime.esomod_last_watered', 'timestamp') | as_datetime() }}
```

DeviceClass: Timestamp
