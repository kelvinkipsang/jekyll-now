---
layout: post
title: Abstraction & Encapsulation,Rival sisters? 
---

Information hiding is not only confused with encapsulation, it is also
often confused with abstraction.

This led to some fanciful speculation on my part. "If encapsulation
could be confused with information hiding," I reasoned, "and
information hiding could also be confused with abstraction, then could
someone argue that abstraction and encapsulation were the same thing?"
Of course, when I said it this way, the argument sounded absurd.

Still, I was curious. I decided to gather a number of different
definitions for abstraction, information hiding, and encapsulation, and
to compare them. This article details what I found.

## ABSTRACTION



	"The essence of abstraction is to extract essential properties
	while omitting inessential details."

		-- [Ross et al, 1975]

	"Abstraction is a process whereby we identify the important
	aspects of a phenomenon and ignore its details."

		-- [Ghezzi et al, 1991]


	"Abstraction is the selective examination of certain aspects of
	a problem. The goal of abstraction is to isolate those aspects
	that are important for some purpose and suppress those aspects
	that are unimportant."

		-- [Rumbaugh et al, 1991]

	"The meaning [of abstraction] given by the Oxford English
	Dictionary (OED) closest to the meaning intended here is 'The
	act of separating in thought'. A better definition might be
	'Representing the essential features of something without
	including background or inessential detail.'"

		-- [Graham, 1991]

	"[A] simplified description, or specification, of a system that
	emphasizes some of the system's details or properties while
	suppressing others. A good abstraction is one that emphasizes
	details that are significant to the reader or user and suppress
	details that are, at least for the moment, immaterial or
	diversionary."

		-- [Shaw, 1984]
    
    
    
Abstraction, as a process, denotes the
extracting of the essential details about an item, or a group of items,
while ignoring the inessential details. Abstraction, as an entity, 
denotes a model, a view, or some other focused representation for an
actual item. Abstraction is most often used as a complexity mastering
technique. For example, we often hear people say such things as: "just
give me the highlights" or "just the facts, please." What these people
are asking for are abstractions.

In short, you might say that abstraction
dictates that some information is more important than other
information, but (correctly) does not specify a specific mechanism for
handling the unimportant information.

## ENCAPSULATION

	"1. to enclose in or as if in a capsule"

		-- [Mish, 1988]

	"The concept of encapsulation as used in an object-oriented
	context is not essentially different from its dictionary
	definition. It still refers to building a capsule, in the case a
	conceptual barrier, around some collection of things."

		-- [Wirfs-Brock et al, 1990]

	"It is a simple, yet reasonable effective, system-building
	tool. It allows suppliers to present cleanly specified
	interfaces around the services they provide. A consumer has full
	visibility to the procedures offered by an object, and no visibility
	to its data. From a consumer's 	point of view, and object is a
	seamless capsule that offers a number of services, with no
	visibility as to how these services are implemented ... The
	technical term for this is encapsulation."

		-- [Cox, 1986]

	"Encapsulation or equivalently information hiding refers to the
	practice of including within an object everything it needs, and
	furthermore doing this in such a way that no other object need ever
	be aware of this internal structure."

		-- [Graham, 1991]

	"We say that the changeable, hidden information becomes the
	secret of the module; also, according to a widely used jargon, we
	say that such information is encapsulated within the implementation."

		-- [Ghezzi et al, 1991]

	"Data hiding is sometimes called encapsulation because the data
	and its code are put together in a package or 'capsule.'"

		-- [Smith, 1991]

	"Encapsulation is used as a generic term for techniques which
	realize data abstraction. Encapsulation therefore implies the
	provision of mechanisms to support both modularity and information
	hiding. There is therefore a one to one correspondence in this
	case between the technique of encapsulation and the principle of
	data abstraction."
  
  
  Like abstraction, the word "encapsulation" can be used to describe
either a process or an entity. As a process, encapsulation means the
act of enclosing one or more items within a (physical or logical)
container. Encapsulation, as an entity, refers to a package or an
enclosure that holds (contains, encloses) one or more items. It is
extremely important to note that nothing is said about "the walls of
the enclosure." Specifically, they may be "transparent," "translucent,"
or even "opaque."

If encapsulation was "the same thing as information hiding," then one
might make the argument that "everything that was encapsulated was also
hidden." This is obviously not true. For example, even though
information may be encapsulated within record structures and arrays,
this information is usually not hidden (unless hidden via some other
mechanism).


One could argue that abstraction is a
technique that helps us identify which specific information should be
visible, and which information should be hidden. Encapsulation is then
the technique for packaging the information in such a way as to hide
what should be hidden, and make visible what is intended to be visible.
