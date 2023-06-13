# Summary
## Piece 1: Audiovisualizer
The first piece I created was an audiovisualizer, which displays a frequency amplitude wave as the song plays. I used Java code (MidiToSynthSequencer.java) to covert a MIDI file to a synthSequencer file that only uses one instrument (SineEnv). I also removed percussion in post (just delete the percussion section in the data.txt output from the Java file). There are two demos in the ./tutorials/synthesis/bin folder, Galaxy.exe and Lake.exe, which showcase this program.
### Galaxy.exe
Song: Arrangement of Gusty Garden Galaxy from Super Mario Galaxy

Original Composer: Koji Kondo

MIDI File: https://www.vgmusic.com/file/98ed5cf946dba46cdcc7b589e87596a8.html
### Lake.exe
Song: Arrangement of Lake from Pokemon Diamond & Pearl

Original Composer: Go Ichinose

MIDI File: https://www.purezc.net/forums/index.php?showtopic=74076
## Piece 2: Piano Roll Interactable
Next, I wanted to create a MIDI piano roll using the AlloLib code. This piece is simply an interactive piano roll, which draws notes at locations based on their frequency and their lengths is is however long the user holds down the key. This piece demonstrates the use of timers to extend the lifespan of a note beyond when the sound of the note end.
### Piano.exe
No composition, just use the keyboard to play some notes (same control scheme as 01_SineEnv_Piano.cpp).
## Piece 3: Piano Roll MIDI
This piece is a non
### Fairy.exe
Song: Arrangement of Great Fairy's Fountain from The Legend of Zelda: Ocarina of Time

Original Composer: Koji Kondo

MIDI Files: https://www.vgmusic.com/file/f1873dccfa37c5232aff5bcf7818c63c.html
## Piece 4: Rhythm Game
### AI Bomb.exe
Song: Artifical Intelligence Bomb

Original Composer: なると

Link: https://www.youtube.com/watch?v=4gtGeZ2wOmo

### Death by Glamour.exe
Song: Death by Glamour from Undertale

Original Composer: Toby Fox

Link: https://www.youtube.com/watch?v=2TgO-tN5wAM
## Tools: MidiParser
