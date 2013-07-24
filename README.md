# What's this for?

During a V-Day in summer 2013, Raj articulated a vision of the VersionOne platform growing to service the needs of 1 million plus users. He emphasized that the platform architecture, and the overall business model, will have to adapt to accomplish this.

One of the first steps in growing our platform capabilities is for us to collectively increase our knowledge about and experience with building highly scalable app architectures.

So, use this repo to share links and ideas about this.

# Greg Young's August 12-14 2013 Visit

Greg Young (of DDD, CQRS, CodeBetter, and SkillsMatter fame) will be coming to V1 in August for 3 days to work with the dev team 
on ramping up on these subjects.

I'm not aware of a specific, hard-set curriculum that Greg will be covering when he visits, but you can get a strong 
sense of what he normally covers from his recurring course outlines here:

• Domain Events, Event Sourcing, and how to apply DDD: http://skillsmatter.com/course/design-architecture/greg-youngs-cqrs-domain-events-event-sourcing-and-how-to-apply-ddd 
•	Advanced CQRS Workshop: http://skillsmatter.com/course/open-source-dot-net/greg-youngs-advanced-cqrs-workshop 
•	Implementing DDD & CQRS with The Event Store: http://skillsmatter.com/event/ajax-ria/event-store-day-nyc

# Getting prepared for Greg's visit

Greg is most well-known for his articulation and elaboration of the Command and Query Responsibility Segregation pattern,
a distributed systems design pattern that extends upon the 
[Command Query Separation](http://en.wikipedia.org/wiki/Command%E2%80%93query_separation) design pattern.

To make the most of Greg's visit, a bunch of us started gathering in **HipChat in CQRSetc** to figure out a plan for 
studying some of Greg and others' materials on CQRS, etc before he arrives.

It's a big subject, as evidenced by this diagram from the [CQRS Journey]((http://msdn.microsoft.com/en-us/library/jj554200.aspx) 
project: 

![CQRS Journey](http://i.msdn.microsoft.com/dynimg/IC610297.png)

## Martin Fowler's summary definition of CQRS

As he often does, Martin Fowler provides a concise, approachable definition of [CQRS](http://martinfowler.com/bliki/CQRS.html):

> CQRS stands for Command Query Responsibility Segregation. It's a pattern that I first heard described by Greg Young. At its heart is a simple notion that you can use a different model to update information than the model you use to read information. This simple notion leads to some profound consequences for the design of information systems.
>
>The mainstream approach people use for interacting with an information system is to treat it as a CRUD datastore. By this I mean that we have mental model of some record structure where we can create new records, read records, update existing records, and delete records when we're done with them. In the simplest case, our interactions are all about storing and retrieving these records.
>
>As our needs become more sophisticated we steadily move away from that model. We may want to look at the information in a different way to the record store, perhaps collapsing multiple records into one, or forming virtual records by combining information for different places. On the update side we may find validation rules that only allow certain combinations of data to be stored, or may even infer data to be stored that's different from that we provide.

## Greg's diagrams

Greg uses these diagrams to depict the "typical CRUD view" on the left side with the CQRS view on the right side:

![CQRS diagram](http://lh3.ggpht.com/_iiRWyargx_M/TIM29FWLpKI/AAAAAAAAAEU/2mBZbTcCXDw/image_thumb1.png?imgmax=1200)

# Study plan outline

Here's what we think, so far:

## Individual Study

We figured we could read / watch the 3 links below individually:

* Fowler's [CQRS summary](http://martinfowler.com/bliki/CQRS.html).
* [CQRS Clarified](http://www.udidahan.com/2009/12/09/clarified-cqrs/) -- Udi Dahan, co-pioneer of the CQRS vision, breaks down a lot of CQRS misconceptions
* [CQRS, Task Based UIs, Event Sourcing agh!](http://codebetter.com/gregyoung/2010/02/16/cqrs-task-based-uis-event-sourcing-agh/) -- Post in which Greg also clarifies a lot of misconceptions
* [CQRS and Event Sourcing -- the Business Perspective](http://skillsmatter.com/podcast/home/greg-young-cqrs-event-sourcing-the-business-perspective) -- Talk where Greg discusses the business perspective on CQRS

## Group Study

* Watch and discuss the recent Pluralsight course over lunch on Tue and Thur in Alph or Loft: ["CQRS Theory and Practice"](http://pluralsight.com/training/Courses/TableOfContents/cqrs-theory-practice), 
from Michael Perry. Course modules are:
 * CAP Theorem
 * Domain Driven Design -- V1's own David Laribee has a great article: [An Introduction to Domain-Driven Design](http://msdn.microsoft.com/en-us/magazine/dd419654.aspx)
 * CQRS
 * Durability
 * Enterprise Service Bus
 * Append Only Models
 * Operational Concerns
 * **Note:** Josh and Ian B have partially completed viewing this course and recommend it.
* Mess around with code samples, such as those listed below.
* TODO: Link to where, why, how V1 eventing code is currently using CQRS-style concepts.
 * And discuss where, how, why it could improve on this.
* Dave highlighted parts of V1 Roadmapping in the HipChat CQRSetc channel on July 10 and said he can do a 3PM on it. 
He also linked to these interviews he's done on DDD, an often closely-related, if not precursory, subject to CQRS:
 * An intro podcast to DDD podcast: http://rubyrogues.com/rr-061-domain-driven-design-ddd-with-david-laribee/
 * Another podcast on DDD: http://deepfriedbytes.com/podcast/episode-6-talking-domain-driven-design-with-david-laribee-part-1/
 * Deep Fried Byes part 2: http://deepfriedbytes.com/podcast/episode-7-talking-domain-driven-design-with-david-laribee-ndash-part-2/

## Extra resources

There are tons of great CQRS resources available. Rinat Abdullin done much to further CQRS, and collected tons of great summary info and detailed links here:

* [CQRS Starting Page](http://abdullin.com/cqrs/)

### More of Greg's recorded free talks

Many of Greg talks are archived for free viewing at his [SkillsMatter Profile](http://skillsmatter.com/expert/home/greg-young)


* Highly recommended: [Assert.That(We.Understand)](http://skillsmatter.com/podcast/home/talk-from-greg-young)
* Highly recommended: [Functional Data Storage](http://skillsmatter.com/podcast/home/greg-young)
* Early presentation at QCON 2008: [Unshackle Your Domain](http://www.infoq.com/presentations/greg-young-unshackle-qcon08)
* 6 hour free course from taught by Greg: [GregYoung CQRS course](http://www.youtube.com/watch?v=whCk1Q87_ZI)
  * Josh "attended" this course and [wrote this review](http://agilefromthegroundup.blogspot.com/2010/09/retrospective-of-greg-youngs-final-cqrs.html). 

### Code Examples

There are lots of samples on the web that have emerged.

* Greg's [Super Simple CQRS](https://github.com/gregoryyoung/m-r) sample is a good intr to Event Sourcing
* Microsoft's Patterns and Practices team underwent a long [CQRS Journey](http://msdn.microsoft.com/en-us/library/jj554200.aspx), aided by more than 100 community collaborators.

### Software

While it's by no means the only option in this namespace, Greg is working on [Event Store](http://www.GetEventStore.com).
