# NTRACES

NTRACES goal is to collect as many stack traces for different kind of windows
behaviours as much as possible, for multiple windows versions, for example 
a stack trace for NTFS Cached File Reads.

The way the traces are generated is that you write a test program, then capture
a stack trace using your favorite method (windbg, sysmon, etc ...), then you
take that trace and submit, currently I am using text files, but I am planning
to put them in a more structured format, and maybe a custom renderer to view 
them in a better way, and a search engine to search through the traces.

The goal is that if you want to know the flow of some functionality, you can look
at the traces, and start looking at these locations, forward or backward as you like.
I also think they might be good to feed into an AI agent to give it some context 
when requested a specific reverse engineering task of a windows functionality.

The project is still in baby-release, like there is only one trace, but I wanted
to at least publish the idea anyways.