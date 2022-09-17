### Hi there 👋

I'm Simon. I'm a professional developer hailing from London in the UK. C# is my go-to language these days (though I am starting to make an attempt to get back into C++). My day job typically involves fairly standard enterprise back-end rigamarole - Web APIs, messaging, cloud platforms, databases, and such. My personal time interests tend to be a little more algorithmic in nature, as is hopefully evidence by the repos you'll find here. Here's an overview of the most interesting public ones:

Testing is important:

* **FlUnit:** A test framework in which tests are defined with a fluent builder. Higher base level of complexity than method-based frameworks, but makes writing succinct, expressive tests (especially parameterised tests) a breeze. No more "arrange, act, assert" comments needed to clarify your test structure, and no more awkward attribute-based test argument retrieval. I use it for all of my other projects, and while its not exactly taking over the world, download counts on NuGet suggest that at least some other people like it too:
  * **[![NuGet version (FlUnit)](https://img.shields.io/nuget/v/FlUnit.svg?style=flat-square)](https://www.nuget.org/packages/FlUnit/) [FlUnit](https://github.com/sdcondon/FlUnit):** The core library.
  * **[![NuGet version (FlUnit.Abstractions)](https://img.shields.io/nuget/v/FlUnit.Abstractions.svg?style=flat-square)](https://www.nuget.org/packages/FlUnit.Abstractions/) [FlUnit.Abstractions](https://github.com/sdcondon/FlUnit.Abstractions):** Shared abstractions between the core library and test adapters
  * **[![NuGet version (FlUnit.VS.TestAdapter)](https://img.shields.io/nuget/v/FlUnit.VS.TestAdapter.svg?style=flat-square)](https://www.nuget.org/packages/FlUnit.VS.TestAdapter/) [FlUnit.Adapters.VSTest](https://github.com/sdcondon/FlUnit.Adapters.VSTest):** Test adapter for VSTest
  
AI and AI-adjacent stuff:

* **[![NuGet version (SCFirstOrderLogic)](https://img.shields.io/nuget/v/SCFirstOrderLogic.svg?style=flat-square)](https://www.nuget.org/packages/SCFirstOrderLogic/) [SCFirstOrderLogic](https://github.com/sdcondon/SCFirstOrderLogic):** Basic but fully functional and documented first-order logic implementations. Based on chapters 8 and 9 of "Artificial Intelligence: A Modern Approach" (Russell &amp; Norvig).
* **[SCPropositionalLogic](https://github.com/sdcondon/SCPropositionalLogic):** Precursor to SCFirstOrderLogic. Basic but fully functional and documents propositional logic implementations. Based on chapter 7 of "Artificial Intelligence: A Modern Approach" (Russell &amp; Norvig).
* **SCGraphTheory:** There are obviously a large number of graph theory implementations out there for .NET. None of them really grabbed me though. In particular, I think graph theory is a domain that benefits greatly from a completely separate abstractions package - and it looks like mine's the only one out there that does this.
  * **[![NuGet version (SCGraphTheory.Abstractions)](https://img.shields.io/nuget/v/SCGraphTheory.Abstractions.svg?style=flat-square)](https://www.nuget.org/packages/SCGraphTheory.Abstractions/) [SCGraphTheory.Abstractions](https://github.com/sdcondon/SCGraphTheory.Abstractions):** Abstractions to facilitate graph algorithms that don't depend on a particular graph representation
  * **[![NuGet version (SCGraphTheory.AdjacencyList)](https://img.shields.io/nuget/v/SCGraphTheory.AdjacencyList.svg?style=flat-square)](https://www.nuget.org/packages/SCGraphTheory.AdjacencyList/) [SCGraphTheory.AdjacencyList](https://github.com/sdcondon/SCGraphTheory.AdjacencyList):** Adjacency list graph implementation
  * **[![NuGet version (SCGraphTheory.Search)](https://img.shields.io/nuget/v/SCGraphTheory.Search.svg?style=flat-square)](https://www.nuget.org/packages/SCGraphTheory.Search/) [SCGraphTheory.Search](https://github.com/sdcondon/SCGraphTheory.Search):** Search algorithms

Gaming is fun:

* **[MyOTKE](https://github.com/sdcondon/MyOTKE):** I got interested in how OpenGL worked at one point, so I made this. A very basic graphics library built on top of the Open toolkit.
* **[SharpFontStandard.Runtimes](https://github.com/sdcondon/SharpFontStandard.Runtimes):** SharpFontStandard** SharpFontStandard is a managed wrapper for [FreeType](http://freetype.org/). For it to work, you obviously need the native libraries at runtime, which it very sensibly doesn't bundle. However, all of the other available packages that provide the native libraries seem to include them as package content, which is entirely the wrong approach, and doesn't work well when the thing that needs it is a library rather than an app. So I made this which does things the right way - by utilising NuGet's support for [runtime dependencies](https://learn.microsoft.com/en-us/nuget/create-packages/supporting-multiple-target-frameworks#architecture-specific-folders).

I'm occasionally moved to create a gist when I come up with or encounter something cool (and small enough to express in gist form):

* **[SqlServerDockerFile](https://gist.github.com/sdcondon/02ac17073e68409f40179f940ac6be77):** Dockerfile for a SQL server instance built to include a database defined in a given SQL script. Created as part of demo-ing an improved (more isolated) E2E testing approach for work.
* **[DacPacDockerFile](https://gist.github.com/sdcondon/1bcc2e4d97903cfff62a0a6827695139): Dockerfile for a SQL server instance built to include a database defined in a given SQL project. Created as part of demo-ing an improved (more isolated) E2E testing approach for work. 
* **[LinqDecomposer](https://gist.github.com/sdcondon/dbbd40903084239221c0c4df2ab2ab7d):** Uses LINQ expressions to decompose and recompose objects, storing each property in a different backing store. Potentially useful when we can store things more efficiently when their decomposed (think spatial indexing). Used by one of my repos that I'm not ready to take public just yet.
* **[ExtensionScripts](https://gist.github.com/sdcondon/338b64dbc3863c9962e89dc399e04e99):** Basic example of using MEF and the Roslyn scripting API to create a scriptable extension system.
* **[Trie](https://gist.github.com/sdcondon/43cfb8ed30f873817d4688c9664a9059):** Generic prefix tree, implementing IDictionary&lt;TKey, TValue&gt;. 
* **[BlockingCollectionBatchPipeline](https://gist.github.com/sdcondon/5be25120916beb6a27189f0cfb173f13):** A simple periodic batching pipeline using BlockingCollections

Old retired stuff that I probably shouldn't bother drawing attention to:

* **[GLHDN](https://github.com/sdcondon/GLHDN):** Same idea as MyOTKE (see above), but using bindings provided by the OpenGL.Net package. Retired it when I realised that OpenTK was bigger and more active.**
* **[SwashbuckleDynamicLocalisation](https://github.com/sdcondon/SwashbuckleDynamicLocalization):** Localisation functionality for Swashbuckle

<!--
**sdcondon/sdcondon** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
