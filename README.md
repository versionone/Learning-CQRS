# What's this for?

During a V-Day in summar 2013, Raj articulated a vision of the VersionOne platform growing to service the needs of 1 million plus users. He emphasized that the platform architecture, and the overall business model, will have to adapt to accomplish this.

One of the first steps in growing our platform capabilities is for us to collectively increase our knowledge about and experience with building highly scalable app architectures.

So, use this repo to share links and ideas about this.

Greg Young (of DDD, CQRS, and CodeBetter, and SkillsMatter fame) will be coming to V1 in August for 3 days to work with the dev team on these subjects.

# First learning op: get prepared for Greg's visit

Greg is most well-known for his articulation and elaboration of the Command and Query Responsibility Segregation pattern.

To make the most of Greg's visit, a bunch of us started gathering in HipChat in CQRSetc to figure out a plan for studying some of Greg and others' materials on CQRS, etc before he arrives.

## Martin Fowler's summary definition of CQRS

As he often does, Martin Fowler provides a concise, approachable definition of [CQRS](http://martinfowler.com/bliki/CQRS.html):

> CQRS stands for Command Query Responsibility Segregation. It's a pattern that I first heard described by Greg Young. At its heart is a simple notion that you can use a different model to update information than the model you use to read information. This simple notion leads to some profound consequences for the design of information systems.
>
>The mainstream approach people use for interacting with an information system is to treat it as a CRUD datastore. By this I mean that we have mental model of some record structure where we can create new records, read records, update existing records, and delete records when we're done with them. In the simplest case, our interactions are all about storing and retrieving these records.
>
>As our needs become more sophisticated we steadily move away from that model. We may want to look at the information in a different way to the record store, perhaps collapsing multiple records into one, or forming virtual records by combining information for different places. On the update side we may find validation rules that only allow certain combinations of data to be stored, or may even infer data to be stored that's different from that we provide.

## Greg's diagrams

Greg uses these diagrams to depict the "typical CRUD view" on the left side with the CQRS view on the right side:

![http://lh3.ggpht.com/_iiRWyargx_M/TIM29FWLpKI/AAAAAAAAAEU/2mBZbTcCXDw/image_thumb1.png?imgmax=800]

## Getting started links

Greg originally articulated CQRS in talks and blog posts like these:

* Blog: [CQRS, Task Based UIs, Event Sourcing agh!](http://codebetter.com/gregyoung/2010/02/16/cqrs-task-based-uis-event-sourcing-agh/)
* Video: [CQRS and Event Sourcing -- the Business Perspective](http://skillsmatter.com/podcast/home/greg-young-cqrs-event-sourcing-the-business-perspective)
* Many of Greg talks are archived for free viewing at his [SkillsMatter Profile](http://skillsmatter.com/expert/home/greg-young)
** Highly recommended: [Assert.That(We.Understand)](http://skillsmatter.com/podcast/home/talk-from-greg-young)
** Highly recommended: [Functional Data Storage](http://skillsmatter.com/podcast/home/greg-young)

Rinat Abdullin has done much to further CQRS, and collected tons of great summary info and detailed links here:

* [CQRS Starting Page](http://abdullin.com/cqrs/)

Udi Dahan co-pioneered the concepts with Greg, and authored many great blog posts, including:

* [CQRS Clarified](http://www.udidahan.com/2009/12/09/clarified-cqrs/) 

Martin Fowler summarized the pattern here:

* [CQRS](http://martinfowler.com/bliki/CQRS.html)

## Study plan outline



TODO: finish this, copy from chat channel

## More resources

TODO: add more links



