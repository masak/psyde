---
title: No comments
---
## In-between transitions

So, I moved my blog home from [use Perl](http://use.perl.org/~masak/journal)
to here. The actual blog posts have already been successfully ported;
see [this post](http://strangelyconsistent.org/blog/its-just-a-tree-silly)
for a bit about the process.

What remains is the comments from the old blog. It's the same trick there,
really. I haven't done it yet because comments weren't part of the minimal
featureset I needed to get the blog going. But they're pretty high on my list.

In summary, here's the plan:

1. Convert the comments from the old blog and put them in place.
2. Create a little form on blog posts, enabling readers to make new comments.

## Waitwait... isn't this site static?

Well, yes. Wouldn't it be a nice little trick to allow comments on a statically
generated blog? I'm sure it's not unheard of.

What I want to do is this. A user types in a comment, using Markdown that
gets rendered in real time as HTML. (stackoverflow uses this, it's a program
called [Showdown](http://attacklab.net/showdown/). I like the idea a lot.) As
the user hits "submit", a message pops up saying "thanks, your comment has
been submitted for review", making it clear that it'll not show up on the
website at once.

Comments that were just made sit in a special quarantine directory waiting to
be reviewed and approved. This could even be done online in some way, and
approved using a login and password. An offline script (invoked manually)
pulls down the approved comments, and makes sure it appears the next time the
blog is regenerated.

That's the plan.
