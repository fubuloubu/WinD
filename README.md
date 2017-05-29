# WinD: WinD is not DOORS - A Friendly Requirements Management Client

WinD is a distributed requirements management tool which allows multiple users to work on large documents together offline. The file format is open and readable, and therefore easily mergeable. The files also allow modular documents (document splitting among multiple files) at the section level through recursive definitions. Object attributes will be extensible through a minimalistic interface that will allow maximal ease of use.

Due to it's distributed nature, auto-incrementing UIDs a la DOORS will be replaced with a UID based on the SHA1 checksum of the object at time of creation. This decision will minimize UID collisions when merging files with other developers.

When ready to export, LaTeX templates are used to control the output format of the document. The resulting document will have be structured for use in a formal environment, and also can show differences between baselined versions using git diff.

Additionally, this program will contain a mergetool for the popular git DVCS, allowing users to merge their edits in a single document with minimal confusion.

IDEAS:
write in expressive logic (LTL/PSL), generate plain-text requirements in human-readable format?
  needs a LUT containing signal->plaintext naming scheme, also for LTL->plaintext. NLG fills in the rest?
needs user-configurable extra fields, but perhaps punt this into a separate product?
