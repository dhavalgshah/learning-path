Source: https://softwareengineering.stackexchange.com/a/263596

A proper answer to your question fills _several books_. I'll come up with a bullet list of buzz words which come into my mind about this, Google and books will do the rest for you.

# Basics
    

-   _Don't go alone_. Try to involve your team-mates as much as possible.
-   _Travel lightweight_.
-   Democracy, but not too much. Sometimes, it's not about what satisfies the biggest number of people, but what hurts the least number of people.
-   Cynefin: Understand your domain - chaotic, complex, complicated, or clear? And beware of confusion.
-   _Keep what_ (needs to be done) _and how_ (it is done) _separate_.
-   Learn about _Scrum_ ("what"), _XP_ (Extreme Programming, "how"), _Kanban_ ("how much", Flow), Lean ("what not") and DevOps ("with whom").
-   _Lean_ is avoiding TIMWOODS, the 8 wastes (Transport, Inventory, Motion, Waiting, Overprocessing, Overproduction, Defects, and Skill), or DOWNTIME (Defects, Overproduction, Waiting, Non-utilized talent, Transportation, Inventory, Motion, Extra processing)
-   _Lean_ also is about _flow_: For overall efficiency, _flow efficiency_ is usually more important than individual efficiency.
-   Learn about _Software Craftsmanship_, _Clean Code_ and _Pragmatic Programming_.
-   Good architecture is about _maximizing the number of decisions not taken_.
-   Scrum / XP / Lean / Agile is about _maximizing the amount of work not done_: _YAGNI_.
-   The _Primary Value of Software_ is that you can _easily change_ it. That it does what it should do is important but that's only its Secondary Value.
-   Prefer an _iterative_ **and** _incremental_ approach, use _time boxes_ for almost everything, especially meetings, make _Parkinson's Law_ your friend because _Hofstadter's Law_ applies.
-   Balance team structure with an understanding of _Conway's Law_ and _Tuckman's Stages of Team Development_.
-   Programming is a quaternity, it is _science_, _engineering_, _art_ and _craft_ all at the same time, and those need to be in balance.
-   Just because _Scrum_ / _XP_ / XYZ is good for someone (including me) doesn't necessarily mean it's good for you / suits your environment. Don't blindly follow the hype, understand it first.
-   _Inspect and Adapt!_ (Scrum Mantra)
-   _Avoid Duplication_ - _Once and only Once!_ (XP Mantra) aka _DRY - Don't Repeat Yourself_ aka _SPOT - Single Point of Truth_

# "What world" work breakdown process
    

-   Collect Requirements as _User Stories_ / _Job Stories_ into a _Product Backlog_.
-   _User_ (of User Story) similar to _Actor_ (in UML) similar to _[Persona](http://www.romanpichler.com/tools/persona-template/)_ similar to _Role_.
-   _Refine User Stories_ until they meet your team's _Definition of Ready_ based on _INVEST_ (Independent, Negotiable, Valuable, Estimable, Small, Testable). (Scrum Meeting: _Backlog Refinement_)
-   Sort the _Product Backlog_ by _Business Value_.
-   Don't start work on a Story before it's _Ready Ready_ (ready according to the definition of ready).
-   Use _Planning Poker_ to estimate the effort of Stories in _Story Points_. Use _Triangulation Comparison_ to ensure consistency of the estimates.
-   The value of estimates isn't the number that comes out. It's the shared understanding.
-   _Yesterday's weather_ is the best estimate, hope the worst.
-   _Split Stories_ if they are too big.
-   Improve delivery culture with a _Definition of Done_.
-   Don't accept the implementation of a User Story before it's _Done Done_ (done according to the Definition of Done).
-   Multiple teams on the same code base should agree on and share the same _Definition of Done_ (especially the _Coding Standards_).
-   Check your progress with _Burndown Charts_.
-   Regularly check with your Stakeholders whether what the team delivers is what's really needed. (Scrum Meeting: _Sprint Review_)

# Story Breakdown
    

-   List and Describe _Users_ / _Personas_ / _Actors_ / _Roles_ (Product Owner)
-   Epic -> Stories (User Story or Job Story) (Product Owner)
-   Story -> Acceptance Criteria (Product Owner)
-   Story -> Subtasks (Dev Team)
-   Acceptance Criteria -> Acceptance Tests (Spec: Product Owner, Impl: Dev Team)
-   Start with a _Walking Skeleton_ which is a minimalistic _End-to-(Half-End)_.
-   Create an _MVP - Minimum Viable Product_.
-   Expand the MVP using _SMURFS - Specifically Marketable, Useful, Releasable Feature Sets_.

# "How world" realization
    

-   Apply the 4 Rules of Simple Design: 1. Passes the tests. 2. Communicates intent. 3. No redundancy. 4. Fewest elements. (And understand why J. B. Rainsberger argues that no redundancy is more important than communicating intent, and why I (Christian Hujer) argue that communicating intent is more important than passing the tests.)
-   Use _OOA/D_, _UML_ and _CRC Cards_, but avoid the _big design upfront_.
-   Implement _object-oriented_, _structured_ and _functional_ at the same time as much as possible, regardless of the programming language.
-   Use _Version Control_ (preferably _distributed_).
-   Start with _Acceptance Tests_.
-   Apply _TDD_, letting the _Three Laws of TDD_ drive you through the _Red-Green-Refactor-Cycle_ in the steps from the _TPP_ (_Transformation Priority Premise_), with _Single-Assert-Rule_, _4 A's_, _GWT (Given When Then)_ from _BDD_.
-   "_Unit Tests_ are _tests which run fast_." — Michael Feathers
-   Apply the _SOLID_ and the _package principles_ to manage _Coupling and Cohesion_. Example: S in SOLID is SRP = Single Responsibility Principle, significantly reduces the number of edit- resp. merge-conflicts in teams.
-   Know _Law of Demeter_ / _Tell, Don't Ask_.
-   Use _Continuous Integration_, if applicable even _Continuous Delivery_ (DevOps).
-   Use _Collective Code Ownership_ based on an agreed common _Coding Standard_ (which should be part of the _Definition of Done_).
-   Apply _Continuous Design Improvement_ (fka Continuous Refactoring).
-   _The Source Code is the Design_. Still upfront thinking is indispensable, and nobody will object a few good clarifying UML diagrams.
-   XP doesn't mean no day is architecture day, it means every day is architecture day. It's a focus on architecture, not a defocus, and the focus is in the code.
-   Keep your _Technical Debt_ low, avoid the five design smells: _Fragility_, _Rigidity_, _Immobility_, _Opacity_, and _Viscosity_.
-   Architecture is about business logic, not about persistence and delivery mechanisms.
-   Architecture is a team sport (_there is no 'I' in Architecture_).
-   _Design Patterns_, _Refactoring_ and the _Transformation Priority Premise_.
-   Project Code is the _ATP-Trinity_ with priorities: 1. _Automation Code_, 2. _Test Code_, 3. _Production Code_.
-   Regularly check with your team peers whether how the team delivers can be improved. (Scrum Meeting: _Sprint Retrospective_)
-   Tests should be _FIRST_ - Fast, Independent, Repeatable, Self-Validating and Timely.

Above list is certainly incomplete, and some parts might even be disputable!

If all this scares you - don't worry, because it _should_ scare you! Succeeding software development projects in teams is not an easy task, and rarely are people properly trained and educated in this art. If this scares you, your intuition is working properly, listen to it. You want to be prepared. Talk to your boss, get some time and training.

# See Also

-   [Who writes the technical 'user stories' in scrum](https://softwareengineering.stackexchange.com/questions/263365/who-writes-the-technical-user-stories-in-scrum/263765#263765)

# Further reading (online)

-   [Portland Pattern Repository](http://c2.com/cgi/wiki?WelcomeVisitors) by Ward Cunningham et al
-   [Principles of OOD](http://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod) by Robert "Uncle Bob" C. Martin
-   [Pragmatic Programmer Tips](https://pragprog.com/the-pragmatic-programmer/extracts/tips)

# Further reading (books)

-   Clean Code by Robert C. Martin
-   Agile Software Development: Principles, Patterns, and Practices by Robert C. Martin
-   The Pragmatic Programmer - From Journeyman to Master by Andrew Hunt and David Thomas
-   Working Effectively with Legacy Code by Michael Feathers
-   Refactoring - Improving the Design of Existing Code by Martin Fowler
-   Refactoring to Patterns by Joshua Kerievsky
-   The Ten Day MBA by Steven Silbiger (sic!)
-   Domain-Driven Design by Eric Evans
-   User Stories Applied by Mike Cohn
-   Object-Oriented Analysis and Design with Applications by Gray Booch et al
-   Design Patterns by the Gang of Four
-   Test Driven Development by Kent Beck
-   Extreme Programming by Kent Beck
-   \[if Java\] Effective Java by Joshua Bloch
