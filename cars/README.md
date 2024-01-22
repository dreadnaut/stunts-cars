# Car files

Cars go in here, under their four-character id directory.

For each car:

- a `<WXYZ>.yaml` file containing
    - important attributes, to be standardised
    - a brief description of the car
- an `images` directory with screenshots or other images of the car
    - limit dimensions to 800×800 or a similar small size?
    - standard names and formats might emerge (e.g., `side.png`)
- a `resources` directory containing all the car files
- an optional `history` directory, containing subdirectories for previous
  versions of the car


## Properties schema

| Propery | Type | Description |
| ---- | ---- | ---- |
| (`id`) | — | The 4-letter identifier for the car is used for the directory and properties file, but it does *not* appear in the file itself |
| `name` | text | The full name of the car |
| `nickname` | text | A shorter, commonly used name for the car |
| `author` | text | The main person credited for designing the car |
| `contributors` | array | Any additional contributors |
| `release_year` | number | Year of release of the first version using this 4-letter identifier |
| `colors` | array | List of liveries, in showroom order; e.g., "Red, Black/Yellow, Red stripes" |
| `urls` | map | Key-value map of related web pages |
| `description` | text | Brief description of the car, should cover all versions with the same 4-letter identifier |
| `game_version` | text | Stunts versions required to use the car; one of `1.0`, or `1.1` |
| `powergear` | text | Type of powergear bug that affects the car; one of `none`, `rigid`, `flexible`, or `negative` |

