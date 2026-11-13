# Doxygen

Doxygen is a tool that produces documentation from source code. It reads specially written comments and turns them into pages describing functions, classes and other parts of a program. This is helpful when a project becomes too large to understand by looking at code alone.

## Documentation comments

In C or C++, Doxygen comments often begin with /** and end with */. A description can be written inside the comment, along with tags that explain specific details.

- \brief gives a short description of a function or class.
- \param describes an input parameter.
- \return explains the returned value.
- \note adds important information.
- \see points to related documentation.
- \author and \version can record author and version details.

For a function add(a, b), the brief description might say that it adds two numbers. There would be one \param entry for a, another for b, and a \return entry describing the sum. Similar comments can be placed before a C++ class and its public methods. Python documentation can use structured docstrings.

## Generating documentation

First, write the comments in the code. Then run doxygen -g Doxyfile to make a configuration file. The Doxyfile controls which sources are processed and which output types are enabled. The command doxygen Doxyfile generates the documentation using those settings.

HTML is convenient for browsing, while LaTeX output can be processed into a PDF manual. Doxygen can also support cross-references and diagrams, including call graphs and inheritance diagrams when the required tools and settings are available. Keeping comments accurate matters because incorrect comments lead to misleading documentation.
