# compact-timezone-list
This package contains an array of timezones based on conventional options found online. It does not follow any complete data set, but all names are according to the tz format: [https://en.wikipedia.org/wiki/List_of_tz_database_time_zones](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones)

More specifically, the fields in the array are:
- `offset`, a string from `"-11:00"` to `"+14:00"` representing the UTC offset
- `label`, a readable label that contains the offset and a longer, descriptive name of the timezone
- `tzCode`, the value from the `tz` standard

## Install

```bash
npm install compact-timezone-list --save
# or
yarn add compact-timezone-list
```

## Example:
```javascript
 import timezones from 'compact-timezone-list';
 // or
 import { minimalTimezoneSet } from 'compact-timezone-list';
```

## Details

- The default export provides a long list of options, with multiple suggestions for each UTC offset.
- The `minimalTimezoneSet` export provides one option per offset type, with a favourite chosen to represent each offset. This is mostly targeted to small, western-focused apps. But, every UTC offset is included.
