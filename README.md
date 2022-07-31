# Home Assistant ZoneMinder core component fork
This is a custom form of the [Home Assistant Zoneminder core component](https://github.com/home-assistant/core/tree/dev/homeassistant/components/zoneminder) that fixes [issue #75724](https://github.com/home-assistant/core/issues/75724) where Zoneminder `ALARM_STATE` was updated from `2` to `3`.

In order to fix the issue, I made a [pull request to zm-py](https://github.com/rohankapoorcom/zm-py/pull/52) python library, used by the Zoneminder core component.

While this pull request is accepted, it is possible to override the Home Assistant core component installing the files on this repository as a custom component. As the fix is actually on the [zm-py](https://github.com/rohankapoorcom/zm-py) library rather than in the component, the library and the fix is included in the custom component.

## Installation
Clone this repository into the `~/config/custom_components/zoneminder` folder of your Home Assistant install. This may imply you have to rename the `zoneminder-hass` folder to `zoneminder`.

# Authors
The Zoneminder core component for Home Assistant and the [zm-py](https://github.com/rohankapoorcom/zm-py) python library are developed by [Rohan Kapoor](https://github.com/rohankapoorcom).
