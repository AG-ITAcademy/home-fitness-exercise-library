# Home Fitness Exercise Library

Find a home fitness exercise and open a video demonstration at its reviewed timestamp. Search by name, alias, equipment or muscle. Bodyweight, dumbbell and kettlebell variations are identified separately.

Provided by Joy2Move, operated by SC GLOBAL PERSPECTIVE SRL. No Joy2Move account, API key or payment is required. This package connects to a public read-only catalog, with no access to profiles, subscriptions or workout history.

## Status

Development package. The Claude-specific endpoint must be deployed before installation works. Claude host playback and directory review are pending; do not interpret local tests as directory approval.

## Test locally

With a current Claude Code installation, from the root of this package:

```sh
claude plugin validate . --strict
claude --plugin-dir .
```

Then ask:

- Show me a kettlebell Romanian deadlift demonstration.
- Show me a wall sit without weights.
- Show me a wall sit and let me choose the equipment.
- Find bodyweight exercises for my core.
- Show me a dead bug demonstration and its full workout.

The tools are `search_exercises` and `get_exercise`. In supported graphical hosts, an interactive card can present the demonstration. Terminal clients can show timestamped YouTube links and links to the exercise page and full workout. Embedded playback is subject to host and YouTube restrictions; direct links remain available.

## Content and limitations

Each demonstration is 15 seconds. Stored timestamps already include a four-second offset from the source chapter. Frame review verifies equipment and timestamp selection, not certified technique or medical suitability. Results are limited to the catalog; unavailable exercises or removed videos must not be invented. This tool cannot diagnose injuries, prescribe rehabilitation, change accounts or take payments.

## Data and support

The remote service receives exercise searches, filters and slugs. It does not store searches in the Joy2Move database. YouTube is contacted when a user plays a demonstration. Website links use `utm_source=claude` without a user or conversation identifier. Hosting providers may process technical request data. See the [privacy policy](https://www.joy2move.net/privacy-policy) and [terms](https://www.joy2move.net/terms).

Support: support@joy2move.net. Report the exercise name and issue, without credentials or medical records.

## Publishing

Source: https://github.com/AG-ITAcademy/home-fitness-exercise-library. Directory submission requires a paid Claude plan and a GitHub connection with write access. The remote MCP connector is submitted separately through the same developer portal.

## License

MIT applies only to this repository's plugin configuration, icon and instructions. The remotely hosted Joy2Move application, exercise catalog and videos are not included and are not licensed under this package's MIT license.
