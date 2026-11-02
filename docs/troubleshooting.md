# Troubleshooting

Work on an approved private copy and back up saves before testing. Change one
setting at a time and record the emulator version and before/after behavior.

- **Game does not launch:** confirm the working-copy path, executable name, and
  mount commands locally; none are assumed by this repository.
- **Display or input problems:** check the exact emulator's manual and test its
  default windowed behavior before changing rendering or input settings.
- **Audio or speed problems:** record symptoms and the current configuration.
  Do not assume a fixed CPU cycle count, sound device, or port is correct.
- **Saves are missing:** confirm which private working directory was used. Do not
  overwrite saves while diagnosing; preserve a separate backup first.
- **Private files appear in Git:** stop before committing. Check the path with
  `git check-ignore -v -- path` and inspect `git status --short --ignored`.
  Ignore rules do not protect files already tracked or explicitly force-added.

When reporting an issue, include the fields in [compatibility](compatibility.md)
and sanitized reproduction steps. Do not attach game files or saves.

Reference: [DOSBox manual](https://www.dosbox.com/DOSBoxManual.html).
