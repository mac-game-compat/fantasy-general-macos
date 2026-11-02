# Local setup

1. Use a legally owned copy of Fantasy General and an emulator obtained separately
   under its own license. This repository supplies neither.
2. Record the game edition and emulator version before testing. No runtime or
   architecture is recommended as verified yet.
3. Obtain explicit approval before inspecting, copying, moving, or changing any
   existing game installation. This bootstrap has not accessed one.
4. From the repository root, create the ignored private workspace before using it
   (this creates empty directories only; it does not access a game installation):

   ```sh
   mkdir -p local/game local/dosbox local/saves local/scratch
   ```

5. After approval, use a private working copy under `local/game/`; preserve the
   original installation and keep independent backups of saves.
6. Copy `config/dosbox.conf.example` to `local/dosbox/dosbox.conf` and review it
   against the documentation for the exact emulator/version you use. Configure
   mounts and the launch command locally only after confirming actual paths and
   executable names. Mount only the intended working directory.
7. Test launch, display, input, audio, and save/load on the working copy; record
   results in `compatibility.md` without uploading game files or saves.

The example targets classic DOSBox configuration syntax. Forks may differ.
It contains no automatic mounts or launch commands. Follow the selected runtime's
manual for its executable path and configuration-loading options; no launcher or
software installation is performed by this project.
