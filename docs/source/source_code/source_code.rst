Source Code
===========
We are in process of improving the source code documentation. Code should be documented using Doxygen syntax.
Many examples exist throughout the codebase.

Example Documentation Blocks
----------------------------

**file.h**

.. code-block:: cpp

    /**
     * @brief Main application entry point.
     * @param argc The number of arguments.
     * @param argv The arguments.
     *
     * @examples
     * main(1, const char* args[] = {"hello", "markdown", nullptr});
     * @end_examples
     */
   int main(int argc, char *argv[]);

.. attention:: The `@examples` and `@end_examples` tags are not standard Doxygen tags. They are custom aliases
   we have specified to simplify documenting examples. Do not confuse this with the standard `@example` tag.

Source
------

Please refer to the `Doxygen Documentation <../doxyhtml/index.html>`_ for more details.

.. todo:: Sphinx and Breathe do not support the Objective-C Domain.
   See https://github.com/breathe-doc/breathe/issues/129

.. .. doxygenindex::
..    :allow-dot-graphs:

.. Ideally, we would use `doxygenfile` with `:allow-dot-graphs:`, but sphinx complains about duplicated namespaces...
