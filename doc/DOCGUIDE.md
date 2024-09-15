# Documentation Style Guide

## A Guide For Writing and Reading KOS' Documentation

### Documentation Structure

KallistiOS uses Doxygen to generate documentation from the project's header files and the following .dox files:

- attribution.dox 
- audio.dox
- debugging.dox
- filesystem.dox
- math.dox
- networking.dox
- peripherals.dox
- system.dox
- threading.dox
- timing.dox
- video.dox

All of them can be found in the doc folder.

#### Topics

Doxygen's documentation is organized in a tree-like structure organized around Topics and Files. In KallistiOS, the previously mentioned list of files describes the top level Topics used to group the corresponding subtopics. As an example, the audio Topic hosts the Driver, Sound Effects and Streaming subtopics. Topics can link to Files and other topics as well. 

#### Files

Files, are (optional) units of documentation that exist under Topics. Doxygen typically uses them to document specific source or header files. In KallistiOS, Files are used to list macros, function signatures, function lists and the headers used in the file.

---

### Documentation Level of Detail

Different levels of detail are provided in KallistiOS' documentation as a way to help the reader quickly find their way through the documentation and the OS. In order to achieve these two goals, documentation should be written with more detail as it gets closer to the File level.

Topic level documentation should aim to inform the reader of what they will find inside it. A top level Topic description must state the API's purpose and hardware it might relate to.

Subtopics are the place to start providing more detailed insights into the API by describing its capabilities and limitations, providing function descriptions and alerting the reader to common pitfalls and known issues. Subtopics that aren't parents to other subtopics should also provide a basic guide into using the API, with a focus on any setup that is required to use it and its key functions.

At the File level, the documentation should focus on describing the inner workings of a module as well as more advanced API usecases and data structures.

#### Linking to Other Pages

---

### Where to Write What