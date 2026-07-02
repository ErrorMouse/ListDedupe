# ListDedupe

ListDedupe is a high-performance, specialized software tool designed to compare, filter duplicates and extract data across multiple text and spreadsheet files. Optimized with a C/C++ core (Cython) and Hash Table algorithms, it processes millions of rows of data in the blink of an eye.

## Core Features & Filtering Modes

The software provides 5 powerful set operations to process two lists of data (Master List - A and Compare List - B):

1. **[D] Duplicates (A ∩ B)**: Extract duplicate data that exists in BOTH the Master and Compare lists. *(Available in Free version)*
2. **[A - B] Master only**: Extract data that ONLY exists in the Master list, removing anything that appears in the Compare list. *(PRO only)*
3. **[B - A] Compare only**: Extract data that ONLY exists in the Compare list, removing anything that appears in the Master list. *(PRO only)*
4. **[AB] Merge All (A ∪ B)**: Merge all data from both lists into a single list, automatically removing any duplicate lines. *(PRO only)*
5. **[AB - D] Unique to both**: Extract "unique" data that appears exactly once (either in Master or in Compare, but not in both). *(PRO only)*

## Supported Input Formats

1. **TXT (Plain Text)**: Each line in the file is treated as a single data entry. *(Available in Free version)*
2. **CSV (Spreadsheet)**: Allows selecting a specific column (A, B, C...) and starting row (1, 2, 3...) to extract exact data regions instead of reading the whole file. *(PRO only)*

## Optimization Options

1. **Sort results (A-Z)**: Automatically sort the result data in alphabetical order. *(Available in Free version)*
2. **Trim spaces**: Automatically remove redundant spaces at the beginning and end of each data line to avoid false mismatches caused by typos. *(PRO only)*
3. **Case-insensitive matching**: Treats "abc" and "ABC" as the same to filter duplicates more accurately. The software uses a smart caching mechanism to KEEP the original capitalization format when exporting results. *(PRO only)*
4. **Split output (>100k lines)**: A safety feature that automatically splits the result file into multiple parts (Part 1, Part 2...) if the results exceed 100,000 lines, preventing the file from crashing Notepad/Excel. *(PRO only)*

## Performance

- Extremely fast processing speed thanks to leveraging Python's native Set data structures, deeply optimized at the OS level. Handles massive file sizes smoothly.
- Modern user interface, high-resolution display support, and completely non-blocking (No "Not Responding" hangs) during calculations thanks to Multi-threading technology.

## Free vs PRO Version

**Free Version Features:**
- [D] Duplicates (A ∩ B) filtering mode.
- TXT file format support.
- Sort results (A-Z) option.

**PRO Version Exclusive Features:**
- All 4 advanced filtering modes ([A - B], [B - A], [AB], [AB - D]).
- CSV file format support with Column/Row selection.
- Trim spaces.
- Case-insensitive matching.
- Split output for large files.
- Hardware-locked license key for security.

## FAQ (Frequently Asked Questions)

**1. I see a blue Windows SmartScreen warning when opening the app. Is it safe?**

> **Important Note:** Since this application is not yet digitally signed, Windows SmartScreen may show a security warning upon the first launch. To proceed, simply click **More info** and then select **Run anyway**. The software is completely safe and will open normally afterwards.

**2. Can I transfer my PRO license to another computer or re-activate it?**

The PRO license is bound to your computer's hardware as an anti-piracy measure. If you need to switch computers or reset your activation, please follow these steps:
1. Go to: [https://customers.freemius.com](https://customers.freemius.com)
2. Log in using the email account that received the license key.
3. Navigate to the **"Licenses"** tab and click **"Deactivate"** for the old machine to free up the slot.
4. Enter the key into the software again and click **"Active"**.