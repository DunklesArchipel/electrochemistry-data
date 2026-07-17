**Changed:**

* Changed lower bound of `svgdigitizer` to v0.14.5.

**Fixed:**

* Fixed ``validate-bib-keys`` crashing with ``UnicodeEncodeError`` on bibliography entries containing UTF-8 characters outside latin-1 (e.g. ``Jović``, ``Adžić``), by escaping such characters as LaTeX sequences before passing them to ``svgdigitizer.pdf.Pdf.build_identifier`` (hotfix for `svgdigitizer#300 <https://github.com/echemdb/svgdigitizer/issues/300>`_).
