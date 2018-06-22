Tilt
====

Tilt is a built-in mode. To enable it, just add the ``tilt`` mode to your machine config list of modes.

Tilt runs at all times, since the machine has to look for slam tilts while games are not running.

Talk about tilt throughs

Ball end events are posted immediately.

```
  switches:
    s_tilt_bob:
        number: 8
        ignore_window_ms: 200
        tags: tilt_warning
  tilt:
    tilt_warning_switch_tag: tilt_warning

    warnings_to_tilt: 3
    reset_warnings_events: ball_ended
    settle_time: 5s
    multiple_hit_window: 300ms
```
