# rename_audio_files
Python script for batch renaming WAV audio files by adding directory-based prefixes, organizing and standardizing naming conventions for audio recordings.

## Usage

Run the script from the command line and provide the audio root  directory using the `--audio_root_directory` (or `-d`) option.

Examples:

```bash
python rename_files.py --audio_root_directory path/to/audio_folder

```

Flags:

- `--audio_root_directory` / `-d`: Path to the folder that contains audio files or subfolders with audio files. (required)
- `--recursive` / `-r`: Search subdirectories recursively to find WAV files (default is True).
- `--verbose` / `-v`: Print progress and summary information (default is True).

Notes:

- If your audio files are organized inside subfolders (e.g., one folder per device), use default `--recursive` value (True) otherwise use False.
- The script only targets files with the `.wav` extension (case-insensitive).
- This code does not add double prefixes on files already having them

