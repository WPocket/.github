
# What is WPocket?
### WPocket is a bundle of distributed computing tools, and WPocket is an acronym for the components that comprise it
* Workhorse
* POW
* O<sup>2</sup>P
* COCA
* Keymaster
* EGAD
* Taskmaster
# What makes WPocket different?
### there are many things that make WPocket different from other Distributed Computing applications
The main thing that WPocket different is that each of the smaller components were designed with working with each other in mind, but are all capable of working independently to some degree.
For example:
- EGAD is an api designed to take multiple different databases and unify all of them under one api interface
- KeyMaster is an API key management utility (requires EGAD)
- Workhorse is a client registration program (might end up being merged with taskmaster)
- TaskMaster is the work queuing program (requires EGAD)
- POW is the proof of work verification system (not required by anything at this moment in time)
- O<sup>2</sup>P is the orchestration layer, combining keymaster, workhorse, and taskmaster in distributing work among open workers
- COCO is your worker, coco instances use config to register with O<sup>2</sup>P using an api key, at which point it then registers as being open to work, after which O<sup>2</sup>P supplies the instance with work (work format is tbd)

both of these are capable of being separated from the dependency chain and run without all the other applications
or you can replace any part of the chain with one of your own, as long as it follows the same standards for communication.

Another thing that makes WPocket different from other solutions is that each of the components were designed with the other in mind, meaning it was built from the groud up with distributed computing and scalability in mind.
