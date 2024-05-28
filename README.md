# README

## Intent

Provide a timeline of public spiritual events as an unordered JSON file.

## Specification

- `title` (required, string) is the name of the event, written as specifically as possible in the past tense.
- `dateInEDTFFormat` (required, string) is the date of the event in Extended Date/Time Format ("EDTF"), [as specified by the Library of Congress](https://www.loc.gov/standards/datetime/). (For example, events that occurred before the common era are written with a `bce` prefix, and events that occurred in our common era are written with a `ce` prefix. Dates are written in `YYYY-MM-DD` format, with `?` characters specifying date components that are approximate or unknown. Seasons are specified with the values `21`, `22`, `23`, `24` to signify 'Spring', 'Summer', 'Autumn', and 'Winter', respectively, in place of a month value (`01` through `12`).)
- `verifiableSourceURLs` (required, array of strings) are URLs of resources that verify the veracity of the date assertion being made. URLs should point as directly as possible to the source verifying the information.
- `artDepictingEventURLs` (optional, array of strings) are URLs of images that depict the event occurring.