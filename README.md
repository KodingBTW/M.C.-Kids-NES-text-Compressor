# M.C.-Kids-NES-text-Compressor

Use same patch nes rom then use:

compressor.py [inFile] [outFile] [outOffset]

Otherwise there are three block of text. Located in:

- 0x4010 to 0x4608
- 0x4609 to 0x4AAB
- 0x4AAC to 0x5082

Some observations:

- It's not quite as space-efficient as whatever the original programmers had, so if you recompress the game's text without any modifications, you'll get a result a few bytes larger than the original compressed data.
- Mixed up some control codes in my previous post: 0x01 clears the text window, while 0x00 ends a string within a block.
 
