# text-file_to_TMX
This script converts a pair of text files containing translations into TMX format.

## Overview
The `text-file_to_TMX` script converts pairs of text files containing source and target language sentences into a Translation Memory eXchange (TMX) file. This file format is widely used in translation tools and systems to manage bilingual translation memories.

The user specifies a directory containing the source and target text files, selects the files to process, provides the source and target language codes, and generates a TMX file. The output TMX file is saved in the same directory as the input files.

See "text-file_to_TMX.PNG" for reference.

## Requirements
- Python 3
- The script uses standard Python libraries (`os`, `xml.etree.ElementTree`), included with the Python installation.

## Files
`text-file_to_TMX.py`

## Usage
1. Prepare the source and target text files with the same number of lines, where each line corresponds to a translation pair.
2. Run the `text-file_to_TMX.py` script.
3. Enter the directory containing the text files when prompted.
4. Select the source and target files from the list displayed by the script.
5. Provide the source and target language codes (e.g., `en` for English, `fr` for French).
6. The script generates a TMX file named `<source_file>_<source_lang>_<target_lang>.tmx` in the same directory.

## Important Note
- The script ensures that the source and target files have the same number of lines. If the line counts do not match, an error will be displayed.
- By default, the script supports `.txt` and commonly used language-specific extensions (e.g., `.en`, `.fr`). Users can dynamically add new extensions during execution.
- TMX files are created using UTF-8 encoding. To modify the encoding, edit the relevant sections in the script.

## License
This project is governed by the CC BY-NC 4.0 license. For comprehensive details, kindly refer to the LICENSE file included with this project.
