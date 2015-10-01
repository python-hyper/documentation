Contributing
============

If you’re reading this you’re probably interested in contributing to one of the
Hyper projects! First, we'd like to say thankyou! Projects like this one
live-and-die based on the support they receive from others, and the fact that
you’re even considering supporting the Hyper project is incredibly generous of
you.

This document lays out general guidelines and advice for contributing to any of
the Hyper projects. If you’re thinking of contributing, start by reading this
thoroughly and getting a feel for how contributing to the project works. If
you’ve still got questions after reading this, please ask us in IRC: we'd be
happy to clarify any questions you may have.

The guide is split into sections based on the type of contribution you’re
thinking of making, with a section that covers general guidelines for all
contributors. Additionally, there is a section to cover our code of conduct,
which applies to all contributions of any kind.

Code Of Conduct
---------------
As contributors and maintainers of this project, and in the interest of
fostering an open and welcoming community, we pledge to respect all people who
contribute through reporting issues, posting feature requests, updating
documentation, submitting pull requests or patches, and other activities.

We are committed to making participation in this project a harassment-free
experience for everyone, regardless of level of experience, gender, gender
identity and expression, sexual orientation, disability, personal appearance,
body size, race, ethnicity, age, religion, or nationality.

Examples of unacceptable behavior by participants include:

- The use of sexualized language or imagery
- Personal attacks
- Trolling or insulting/derogatory comments
- Public or private harassment
- Publishing other's private information, such as physical or electronic
  addresses, without explicit permission
- Other unethical or unprofessional conduct.

Project maintainers have the right and responsibility to remove, edit, or
reject comments, commits, code, wiki edits, issues, and other contributions
that are not aligned to this Code of Conduct. By adopting this Code of Conduct,
project maintainers commit themselves to fairly and consistently applying these
principles to every aspect of managing this project. Project maintainers who do
not follow or enforce the Code of Conduct may be permanently removed from the
project team.

This code of conduct applies both within project spaces and in public spaces
when an individual is representing the project or its community.

Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by opening an issue or contacting one or more of the project
maintainers.

This code of conduct applies to all Hyper projects. This code of conduct is
adapted from `version 1.2.0`_ of the `Contributor Covenant`_.

.. _version 1.2.0: http://contributor-covenant.org/version/1/2/0/
.. _Contributor Covenant: http://contributor-covenant.org

All Contributions
-----------------

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

The maintainers of the specific sub-project have the last word on whether or
not a contribution is suitable for that project. All contributions will be
considered, but from time to time contributions will be rejected because they
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
system. This will automatically run the tests against any pull request raised
against any ``hyper`` repository. The continuous integration system treats a
regression in code coverage as a failure of the test suite.

Before a contribution is merged it must have a green run through the CI system.

.. _tox: http://tox.readthedocs.org/en/latest/

Code Review
~~~~~~~~~~~

Contributions will not be merged until they've been code reviewed. You should
implement any code review feedback unless you strongly object to it. In the
event that you object to the code review feedback, you should make your case
clearly and calmly. If, after doing so, the feedback is judged to still apply,
you must either apply the feedback or withdraw your contribution.

New Contributors
~~~~~~~~~~~~~~~~

If you are new or relatively new to Open Source, welcome! The Hyper project
aims to be a gentle introduction to the world of Open Source. If you're
concerned about how best to contribute, please consider mailing a maintainer or
asking for help on IRC.

Please also check the :ref:`early-feedback` section.

Documentation Contributions
---------------------------

Documentation improvements are always welcome! The documentation files for
individual projects live in the ``docs/`` directory of the codebase for that
project, and the general documentation for the project as a whole live in the
`documentation`_ repository. They're written in `reStructuredText`_, and use
`Sphinx`_ to generate the full suite of documentation.

When contributing documentation, please attempt to follow the style of the
documentation files. This means a soft-limit of 79 characters wide in your text
files and a semi-formal prose style.

.. _reStructuredText: http://docutils.sourceforge.net/rst.html
.. _Sphinx: http://sphinx-doc.org/index.html
.. _documentation: https://github.com/python-hyper/documentation


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
