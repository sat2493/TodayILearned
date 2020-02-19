# Compartmentalization

TIL that compartmentalizing your main dart components can be achieved through outsourcing it to different files.

Rather than containing all your classes in a single dart file, it's better to have a single widget per file. This not only makes code easier to maintain, but it makes the runtime of our application much faster. Particularly for rebuild processes.
