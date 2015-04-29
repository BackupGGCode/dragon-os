Executables will only be executed under the following conditions:
  * The executable is of ELF format (or another supported format) with a machine type equivalent of what the machine is able to execute.
  * The executable must be approved for execution by a kernel module.

The default ``Kernel Module for Execution'' (KME) will check a database (stored in a secure location on the OS install media) for a list of hash keys of known safe executables. Executables may be added to the user's local list and application developers may submit executables to AxioSoft for approval. When new executables are added, the list database will be updated on an AxioSoft server. The OS' KME may then download this list. Those who make custom distributions of the OS may supply their own KME. This is especially true for home entertainment system vendors who may wish to enforce a proprietary or protected design. (For example, those that wish to make sure that games were licensed for the console.)
