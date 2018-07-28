Hello everyone!

This is my video pitch for Pysangamam 2018.

I would be covering "Engineering Documentation for scientific python".

Documentation is one of the biggest obstacles in sharing code in an techincal group or organisation.

Misisng docs, incomplete docs, obsolete docs are some of the biggest issues developers face. In this talk, we cover what constitues bad documentation, the impact of poor documentation, and a hawk eye perspective to address this. 

In specific, we talk about both cultural and tooling changes neeeded, that is, a bottoms-up and a top-down approach. 

This talk is more oriented to the bulk of development that occurs in scientific python, but you may find the overall idea tailorable for your specific application. 

In order to address this issue of bad documentation, we propose a simplistic notion of integrating documentation effectively with code workflow. The main idea is to stop "inflicting help" and seperate source from presentation. Let's keep documentation as simple as it can be.

We show how we can let developers focus more on the source and a uniform style of documentation in code. We achieve this by abstracting the remaining need of formatting as well as serving docs.

The net result is that you no longer have to worry about updating any wiki's or google sites. Neither do you have to worry about the complexity styling guidelines with tools like Sphinx or doxygen, you design your own barebones convention. Plus, if you use any version controlling tool like git, this readily fits into your existing workflow. 

One of our goals was to ensure docs can be readable both on a service like github or gitlab, and also on a rendered site that you would use. To do this, we utilise the markdown format on the developer end, in a predictable location for every repository or codebase you would use.

To scale this system, we identify two main components of documentation - extracting API and generic documentation, and second, serving them. Both of these can be adapted to different use cases, at a variety of scales.

At the end of the talk, we demonstrate this with an example of building your own documentation pipeline and conclude with our implementation of such a pipeline, the impact it has had in our organisation and some future goals. 



