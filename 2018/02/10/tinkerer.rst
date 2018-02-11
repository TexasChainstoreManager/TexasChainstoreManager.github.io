============
Tinkerer
============

I'm writing this blog using a tool called `Tinkerer <http://tinkerer.me>`_.

It's a blogging system created with Pythonistas in mind.

It feels very familiar. You simply ``pip install tinkerer`` and use
the commandline tool ``tinker`` to publish blog posts and web pages
written in `ReStructuredText <http://docutils.sourceforge.net/docs/user/rst/quickstart.html>`_.

Blog posts are created using ``tinker --post``.

Pages are created using ``tinker --page``.

This creates source that is built into HTML using ``tinker --build``.

And that's pretty much all there is to it!

Hosting
=========

I had originally considered WordPress, just because I've heard of
it and it's really popular, but I didn't want to host something
dynamic just to write a blog. I'm aware of the cost difference
in running an AWS EC2 instance vs. serving static content using S3!

Luckily Tinkerer suggests an even easier solution, and free! Hosting your 
page on GitHub. GitHub does some magic where a repo named 
``${USERNAME}.github.io`` gets hosted at ``https://${USERNAME}.github.io``. 
This is great because you don't need to separately store your repo and 
publish your site.

.. author:: default
.. categories:: none
.. tags:: markup,rst,restructuredtext,tinkerer,python,hosting,github
.. comments::
