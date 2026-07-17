**Changed:**

* Changed lower bound of `svgdigitizer` to v0.14.5.
* Changed metadata-schema version (``mdstools`` git tag and ``SCHEMA_VERSION``) from 0.8.2 to 0.8.3 and flipped the ``click`` pin from ``<8.2`` to ``>=8.2`` (required by ``linkml`` 1.11.1, on which ``mdstools`` 0.8.3 depends).

**Fixed:**

* Fixed ``validate-bib-keys`` crashing with ``UnicodeEncodeError`` on bibliography entries containing UTF-8 characters outside latin-1 (e.g. ``Jović``, ``Adžić``), by escaping such characters as LaTeX sequences before passing them to ``svgdigitizer.pdf.Pdf.build_identifier`` (hotfix for `svgdigitizer#300 <https://github.com/echemdb/svgdigitizer/issues/300>`_).
