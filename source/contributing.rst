Contributing
============

If you’re reading this, you’re probably interested in contributing to one of the
Hyper projects! First, we'd like to say thank you! Projects like this one
live-and-die based on the support they receive from others, and the fact that
you’re even considering supporting the Hyper project is incredibly generous of
you.

This document lays out general guidelines and advice for contributing to any of
the Hyper projects. If you’re thinking of helping, start by reading this
thoroughly and getting a feel for how the project works. If
you’ve still got questions after reading this, please ask us in IRC: we'd be
happy to clarify any questions you may have.

We've organized this guide into sections:

- our code of conduct, which applies to all contributions of any kind
- general guidelines for all contributors
- specific information based on the type of contribution you’re
  thinking of making
       - code contributions
       - documentation
       - bug reports
       - feature requests

Code Of Conduct
---------------

The following code of conduct applies to all projects that are under the
umbrella of the hyper project.

Our Pledge
~~~~~~~~~~

In the interest of fostering an open and welcoming environment, we as
contributors and maintainers pledge to making participation in our project and
our community a harassment-free experience for everyone, regardless of age,
body size, disability, ethnicity, gender identity and expression, level of
experience, nationality, personal appearance, race, religion, or sexual
identity and orientation.

Our Standards
~~~~~~~~~~~~~

Examples of behavior that contributes to creating a positive environment
include:

- Using welcoming and inclusive language
- Being respectful of differing viewpoints and experiences
- Gracefully accepting constructive criticism
- Focusing on what is best for the community
- Showing empathy towards other community members

Examples of unacceptable behavior by participants include:

- The use of sexualized language or imagery and unwelcome sexual attention or
  advances
- Trolling, insulting/derogatory comments, and personal or political attacks
- Public or private harassment
- Publishing others' private information, such as a physical or electronic
  address, without explicit permission
- Other conduct which could reasonably be considered inappropriate in a
  professional setting

Our Responsibilities
~~~~~~~~~~~~~~~~~~~~

Project maintainers are responsible for clarifying the standards of acceptable
behavior and are expected to take appropriate and fair corrective action in
response to any instances of unacceptable behavior.

Project maintainers have the right and responsibility to remove, edit, or
reject comments, commits, code, wiki edits, issues, and other contributions
that are not aligned to this Code of Conduct, or to ban temporarily or
permanently any contributor for other behaviors that they deem inappropriate,
threatening, offensive, or harmful.

Scope
~~~~~

This Code of Conduct applies both within project spaces and in public spaces
when an individual is representing the project or its community. Examples of
representing a project or community include using an official project e-mail
address, posting via an official social media account, or acting as an
appointed representative at an online or offline event. Representation of a
project may be further defined and clarified by project maintainers.

Enforcement
~~~~~~~~~~~

Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting the project team `by email`_. All complaints will be
reviewed and investigated and will result in a response that is deemed
necessary and appropriate to the circumstances. The project team is obligated
to maintain confidentiality with regard to the reporter of an incident.
Further details of specific enforcement policies may be posted separately.

Project maintainers who do not follow or enforce the Code of Conduct in good
faith may face temporary or permanent repercussions as determined by other
members of the project's leadership.

Attribution
~~~~~~~~~~~

This Code of Conduct is adapted from the `Contributor Covenant`_, version 1.4,
`available here`_.

All Contributions
-----------------

.. _early-feedback:

Get Early Feedback
~~~~~~~~~~~~~~~~~~

If you are contributing, do not feel the need to sit on your contribution until
it is perfectly polished and complete. It helps everyone involved for you to
seek feedback as early as you possibly can. Submitting an early, unfinished
version of your contribution for feedback in no way prejudices your chances of
getting that contribution accepted, and can save you from putting a lot of work
into a contribution that is not suitable for the project.

Contribution Suitablility
~~~~~~~~~~~~~~~~~~~~~~~~~

The maintainers of a sub-project have the last word on whether or
not a contribution is suitable for that project. We consider all contributions,
but from time to time contributions will be rejected because they
do not suit the project.

If necessary, a contributor should feel free to ask maintainers of other hyper
projects to adjudicate, especially if they feel their contribution is being
unfairly discriminated against.

If your contribution is rejected, don’t despair! So long as you followed these
guidelines, you’ll have a much better chance of getting your next contribution
accepted.

Code Contributions
------------------

When contributing code, you’ll want to follow this checklist:

1. Fork the repository for the project in question on GitHub.
2. Run the tests to confirm they all pass on your system. If they don’t, you’ll
   need to investigate why they fail. If you’re unable to diagnose this
   yourself, raise it as a bug report by following the guidelines in this
   document: :ref:`bug-reports`.
3. Write tests that demonstrate your bug or feature. *Ensure that they fail*.
4. Make your change.
5. Run the entire test suite again, confirming that all tests pass *
   including the ones you just added*.
6. Send a GitHub Pull Request containing your changes. GitHub Pull Requests are
   the expected method of code collaboration on this project. If you object to
   the GitHub workflow, you may mail a patch to one of the project maintainers.

The following sub-sections go into more detail on some of the points above.

Tests & Code Coverage
~~~~~~~~~~~~~~~~~~~~~

All Hyper projects have a substantial suite of tests, both unit tests and
integration tests, and have 100% code and branch coverage. Whenever you
contribute, you must write tests that exercise your contributed code, and you
must not regress the code coverage.

To run the tests, you need to install `tox`_. Once you have, you can run the
tests against all supported platforms by simply executing ``tox``.

If you're having trouble running the tests, please consider raising a bug
report using the guidelines in the :ref:`bug-reports` section.

If you've done this but want to get contributing right away, you can take
advantage of the fact that all Hyper projects use a continuous integration
system. This system will automatically run the tests against any pull request
raised against any Hyper repository. The continuous integration system treats
a regression in code coverage as a failure of the test suite.

Before a contribution is merged, it must have a green run through the CI system.

.. _tox: http://tox.readthedocs.org/en/latest/

Code Review
~~~~~~~~~~~

Contributions will not be merged until they've been code reviewed. You should
implement any code review feedback unless you strongly object to it. If
you object to the code review feedback, you should make your case
clearly and calmly. If, after doing so, the feedback is judged to apply still,
you must either incorporate the feedback or withdraw your contribution.

New Contributors
~~~~~~~~~~~~~~~~

If you are new or relatively new to Open Source, welcome! The Hyper project
aims to be a gentle introduction to the world of Open Source. If you're
concerned about how best to contribute, please consider mailing a maintainer or
asking for help on IRC.

Please also check the :ref:`early-feedback` section.

Security
~~~~~~~~

We have a security policy we take very seriously. Please read :doc:`security`
for more details.

Documentation Contributions
---------------------------

Documentation improvements are always welcome! The documentation files for
individual projects live in the ``docs/`` directory of the codebase for that
project, and the general documentation for the project as a whole live in the
`documentation`_ repository. They're written in `reStructuredText`_, and use
`Sphinx`_ to generate the full suite of documentation.

When contributing documentation, please attempt to follow the style of the
documentation files. Use a soft-limit of 79 characters wide in your text
files and a semi-formal prose style.


.. _bug-reports:

Bug Reports
-----------

Bug reports are hugely important! Before you raise one, though, please check
through the GitHub issues for that project, **both open and closed**, to
confirm that the bug hasn't been reported before. Duplicate bug reports are a
huge drain on the time of other contributors, and should be avoided as much as
possible.


Feature Requests
----------------

Feature requests are always welcome, but please note that all the general
guidelines for contribution apply. Also note that the importance of a feature
request *without* an associated Pull Request is always lower than the
importance of one *with* an associated Pull Request: code is more valuable than
ideas.


.. _by email: mailto:cory@lukasa.co.uk
.. _Contributor Covenant: http://contributor-covenant.org
.. _available here: http://contributor-covenant.org/version/1/4/
.. _reStructuredText: http://docutils.sourceforge.net/rst.html
.. _Sphinx: http://sphinx-doc.org/index.html
.. _documentation: https://github.com/python-hyper/documentation
