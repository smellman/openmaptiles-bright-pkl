# OSM Bright style written in Pkl language

This is a fork of the [OSM Bright style](https://github.com/openmaptiles/osm-bright-gl-style) that has been converted to the [Pkl language](https://pkl-lang.org/index.html).

## How to use

To use this style, you need to convert it to the GL JSON format. You can do this by running the following command:

```bash
pkl eval -f json style.pkl > style.json
```

## How to validate

To validate the style, you can run the following command:

```bash
pkl eval -f json style.pkl | gl-style-validate
```

Or zsh:

```zsh
gl-style-validate <(pkl eval -f json style.pkl)
```

Also you need install 'gl-style-validate' command:

```bash
npm install @maplibre/maplibre-gl-style-spec --global
```

## License

The code in this repository is licensed under the BSD 3-Clause License.

The design of the style is licensed under the CC-BY 4.0 License.
