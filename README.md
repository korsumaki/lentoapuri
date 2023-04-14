# Lentoapuri #

HTML5 application for creating Flight Plans in Finland.

The aim is to fill official flight plan form based on what application knows about airfields, users location and some users selections.

Live version is available in [www.lentoapuri.fi/](https://www.lentoapuri.fi/ "Lentoapuri").

## Unit tests ##

Unit tests are using [QUnit framework](https://qunitjs.com/).
- Test source: [scripts/tests.js](scripts/tests.js "tests.js")
- Test execution: [www.lentoapuri.fi/test.html](https://www.lentoapuri.fi/test.html "Lentoapuri Unit tests")

## File encoding for data files ##

It could be that data files are opened with wrong encoding in VS Code and Scandinavian letters are not presented correctly.

To open with correct encoding:
1. Click current encoding name e.g. `Windows 1255` or `UTF-8` from bottom bar of VS Code
2. Select action `Reopen with Encoding`
3. Select `ISO 8859-1`

## Data file conversions ##

Some data files can be converted from raw data to json. Raw file format is somewhat copy-paste from AIP.

### Airspace conversion to json file ###

- Update raw data file [data/airspace-raw.txt](data/airspace-raw.txt)
- Open [airspace-conv.html](airspace-conv.html) in browser. Try online [www.lentoapuri.fi/airspace-conv.html](https://www.lentoapuri.fi/airspace-conv.html "Airspace conversion")
- Copy paste json output to destination datafile (from beginning of the file until log area begin)

### Estonian aerodrome conversion to json file ###

- Update raw data file [data/EE-aerodromes-raw.txt](data/EE-aerodromes-raw.txt)
- Open [aerodrome-conv.html](aerodrome-conv.html) in browser. Try online [www.lentoapuri.fi/aerodrome-conv.html](https://www.lentoapuri.fi/aerodrome-conv.html "Estonian aerodrome conversion")
- Copy paste json output to destination datafile (from beginning of the file until log area begin)
