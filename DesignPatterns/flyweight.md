In# tent
* Use sharing to support large numbers of fine-grained objects efficiently.
* The Motif GUI strategy of replacing heavy-weight widgets with light-weight gadgets.

# Problem
* Designing objects down to the lowest levels of system "granularity" provides optimal flexibility, but can be unacceptably expensive in terms of performance and memory usage.



# Check list
* Ensure that object overhead is an issue needing attention, and, the client of the class is able and willing to absorb responsibility realignment.
* Divide the target class's state into: shareable (intrinsic) state, and non-shareable (extrinsic) state.
* Remove the non-shareable state from the class attributes, and add it the calling argument list of affected methods.
* Create a Factory that can cache and reuse existing class instances.
* The client must use the Factory instead of the new operator to request objects.
* The client (or a third party) must look-up or compute the non-shareable state, and supply that state to class methods.

Rules of thumb
* Whereas Flyweight shows how to make lots of little objects, Facade shows how to make a single object represent an entire subsystem.
* Flyweight is often combined with Composite to implement shared leaf nodes.
* Terminal symbols within Interpreter's abstract syntax tree can be shared with Flyweight.
* Flyweight explains when and how State objects can be shared.


http://3.bp.blogspot.com/-Tz2wNYNSJDE/UpA-pPhPypI/AAAAAAAAAwo/PCmcc4d2GNk/s1600/Flyweight+Design+Pattern.JPG




https://sourcemaking.com/files/v2/content/patterns/Flyweight_example1.svg
http://2.bp.blogspot.com/_GuPw-7YN_ko/S_fHQ8otQ8I/AAAAAAAAA7g/r8b1BeGwV3w/s1600/Slide7.JPG
http://image.slidesharecdn.com/03compositeandflyweightpattern-100729035033-phpapp01/95/design-patterns-03-composite-and-flyweight-pattern-11-728.jpg?cb=1280375886
http://image.slidesharecdn.com/04-structuralpatterns-140618172640-phpapp02/95/patterns04-structural-design-patterns-19-638.jpg?cb=1403116772
