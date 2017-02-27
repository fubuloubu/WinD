# WinD
WinD is not DOORS - A Friendly Requirements Management Client

WinD is a requirements management tool developed as a JS/HTML5 application which allows multiple users to work on large documents in parallel. The file format WinD uses leverages JSON notation which is easily mergeable via any VCS. The files will allow modular documents (document splitting among multiple files) at the section level through recursive definitions. Object attributes will be extensible through a minimalistic interface that will allow maximal ease of use.

Additionally, this program will contain a mergetool for the popular git DVCS, allowing users to merge their edits in a single document with minimal confusion.

Due to it's distributed nature, auto-incrementing UIDs a la DOORS will be replaced with a UID based on the SHA1 checksum of the object at time of creation. This decision will minimize UID collisions when merging files with other developers.

When ready to export, LaTeX templates are used to control the output format of the document. The resulting document will have be structured for use in a formal environment, and also can show differences between baselined versions using git diff.

