# Home Fitness Exercise Library

Find a home fitness exercise and open a video demonstration at its reviewed timestamp. Search by name, alias, equipment or muscle. Bodyweight, dumbbell and kettlebell variations are identified separately.

Provided by Joy2Move, operated by SC GLOBAL PERSPECTIVE SRL. No Joy2Move account, API key or payment is required. This package connects to a public read-only catalog, with no access to profiles, subscriptions or workout history.

## Status

The public Claude endpoint is live. Search and interactive exercise cards have been tested in Claude. The Mux playback update requires deployment and a final test in Claude before submission. Directory review is pending; this is not yet an approved directory listing.

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

The tools are `search_exercises` and `get_exercise`. Claude shows an interactive exercise card with equipment details and links to the demonstration, exercise page and full workout. The Claude card uses Mux for inline playback at the reviewed timestamp and pauses after 15 seconds. A timestamped YouTube link remains as a fallback if inline playback is unavailable; external YouTube playback continues normally. ChatGPT continues to use its existing YouTube player. Terminal clients show timestamped links. No browser security settings need to be changed.

## Content and limitations

Each demonstration is 15 seconds. Stored timestamps already include a four-second offset from the source chapter. Frame review verifies equipment and timestamp selection, not certified technique or medical suitability. Results are limited to the catalog; unavailable exercises or removed videos must not be invented. This tool cannot diagnose injuries, prescribe rehabilitation, change accounts or take payments.

## Data and support

The remote service receives exercise searches, filters and slugs. It does not store searches in the Joy2Move database. Mux is contacted when a user plays an inline demonstration in Claude. YouTube is contacted only when the user follows the YouTube fallback link. Website links use `utm_source=claude` without a user or conversation identifier. Hosting providers may process technical request data. See the [privacy policy](https://www.joy2move.net/privacy-policy) and [terms](https://www.joy2move.net/terms).

Support: support@joy2move.net. Report the exercise name and issue, without credentials or medical records.

## Publishing

Source: https://github.com/AG-ITAcademy/home-fitness-exercise-library. Directory submission requires a paid Claude plan and a GitHub connection with write access. The remote MCP connector is submitted separately through the same developer portal.

## License

MIT applies only to this repository's plugin configuration, icon and instructions. The remotely hosted Joy2Move application, exercise catalog and videos are not included and are not licensed under this package's MIT license.
