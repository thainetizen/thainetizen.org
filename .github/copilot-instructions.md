## General

- [ ] Do not commit to Git or post on issues/PRs a content containing
      any personal or sensitive information,
      including citizen ID number, security key and passwords.
- [ ] Be very careful about web security when doing any configuration,
      or writing/suggesting a code.
- [ ] Base URL of the website is https://thainetizen.org
- [ ] Use a very concise and meaningful URL for pages.
- [ ] The website primary language is Thai.
      Some pages may have English translation.

## Units / Locale

- [ ] The main audience is for people in Thailand.
- [ ] Use the metric system for all measurements.
- [ ] Temperature: Use degrees Celsius (°C).
- [ ] Currency: Use Thai Baht as the primary currency.
      with Euros (€) and US Dollars (USD) provided in parentheses
      for convenience.
      Action Item: Recheck the current €/USD exchange rate for accuracy.
- [ ] Timezones: Use UTC+7 in text meant for human consumption.

## General language use

- [ ] Prefer clear, concise, and unambiguous sentences.
- [ ] Avoid words and phrases that may have more than one interpretation.
- [ ] Avoid overly long paragraphs. Breaking up text into smaller paragraphs,
      using bullet points, or creating numbered lists to improve readability.
- [ ] Help reader's comprehension by separating distinct concepts, processes,
      criteria, or categories.
- [ ] Use parallel language structures in lists and documentation.
- [ ] Use a uniform writing style, particularly when presenting similar or
      related information, so the reader's compare easily.
- [ ] If not specified otherwise, use Chicago style for reference/citation.
- [ ] When writing on level of requirements, use the verbal forms consistently.
      Use either ISO/IEC verbal form (ISO/IEC Directives, Part 2 --
      Principles and rules for the structure and drafting of ISO and IEC
      documents) or IETF verbal form (RFC 2119 and RFC 8174).
      Try to detect the level of requirements from type/domain of the document.
      IETF is default for internet/web/semantic web projects in general.
      ISO is default for SPDX project.
- [ ] Use either American or British spelling consistently.
      Check for inconsistency.
      If not specified, or there is no clear existing example in the file or
      the repo, use British spelling as a default.

## Naming conventions

- [ ] Follow standard naming conventions for the programming language
      and framework you are using.
- [ ] For URLs/IRIs, use lowercase letters and hyphens to separate words
      (e.g., `my-api-endpoint`) and follow W3C Cool URIs for the Semantic Web:
      https://www.w3.org/TR/cooluris/
- [ ] Consult Schema.org vocabularies when deciding about names.
- [ ] Consult "Style Guidelines for Naming and Labeling Ontologies in the
      Multilingual Web" https://www.researchgate.net/publication/277224472

## Tidy code and documentation

- [ ] Ensure that the code is well-formatted and adheres to the style
      guidelines of the programming language you are using.
- [ ] Use linters and formatters where applicable.
- [ ] Use "sentence case" for headings and titles in documentation.
- [ ] Write clear and concise comments and documentation for your code.
      For something obvious, avoid comments that just restate the code.
- [ ] After making changes, review the code and documentation to ensure
      up-to-dateness, correctness, consistency, and clarity.
- [ ] Make sure that all code comments, APIs, and documentation are consistent
      with the current state of the codebase.
- [ ] Make sure that the examples in the documentation are runnable, up-to-date
      and reflect the current behavior of the code.      

## File header

- [ ] When possible, put relevant SPDX File Tags at source code header,
      using appropriate comment marker for the programming language or
      markup language.
      See https://spdx.github.io/spdx-spec/v2.3/file-information/
  - [ ] SPDX-FileContributor
  - [ ] SPDX-FileCopyrightText
  - [ ] Default SPDX-FileType for code is "SOURCE"
  - [ ] Default SPDX-FileType for documentation is "DOCUMENTATION"
  - [ ] Default SPDX-License-Identifier for code is "Apache-2.0"
  - [ ] Default SPDX-License-Identifier for documentation is "CC0-1.0"
  - [ ] Sort SPDX metadata.

## Shell scripts and command line

- [ ] Mind the differences between GNU, BSD, macOS,
      and other implementations of common Unix tools.
- [ ] Be defensive on variable expansion.
- [ ] Use quotes or other constructs to encapsulate paths, make it compatible
      with different kinds of shells.
- [ ] Be mindful about semantic of different types of quotation marks.

## Library imports and dependencies

- [ ] Recheck the correctness of library/module/package name.
      Be very careful of slopsquatting and typosquatting attacks.
- [ ] Use the most updated version of the library that is supported
      by the OS/compiler/framework currently being in used.
- [ ] In source code, sort imports by the programming language convention
      and then by alphabetical order whenever possible.
      Be careful of specific order of import requirements of some dependencies.
- [ ] In build metadata (like pyproject.toml in Python) or
      dependency list (like requirements.txt in Python), sort dependencies.
- [ ] Warn users about abandoned dependency with no maintenance
      for long time and suggest equivalent drop-in replacement.

## API

- [ ] The over architecture, code, API endpoints to follow the latest version
      of OpenAPI specification at https://spec.openapis.org/oas/
- [ ] API endpoints must use proper HTTP return code
- [ ] Follows web best practices as recommended by OpenAPI, IETF, W3C, etc.

## JSON

- [ ] When serialize to JSON, always enclose decimal values
      (for example, xs:decimal) in quotes to guarantee correct type
      interpretation and preserve precision.
- [ ] Make sure JSON is valid and well-formatted.

## Markdown

- [ ] When including metadata in Markdown file,
      put them as YAML between triple-dashed lines,
      as used by Hugo and Jekyll front matter.
- [ ] Be strict on the Markdown formatting.
      Be mindful that what works on GitHub may not work on MkDocs, for example.
      Ty to keep with the standard Markdown.
- [ ] Use Markdownlint to detect and fix malformatted.

## Diagram

- [ ] When draw the diagram in ASCII/text, recheck if all the lines are well
      aligned.
      Count the characters and adjust the spaces so the lines align well.

## HTML

- [ ] Make sure HTML is valid and well-formatted.
- [ ] Make sure there is no trailing whitespace in the HTML file.
- [ ] Be conscious about accessibility. Consider to follow W3C web
      accessibility recommendations when possible.
- [ ] Use sensible and concise element IDs and names that allow code
      readability, name grouping also helps.

## CSS

- [ ] Make sure there is no unused styles.
- [ ] Use sensible and concise element IDs and names that allow code
      readability, name grouping also helps.

## Version

- [ ] When suggest dependencies, recheck the version; if the version exists,
      or if the version compatible with the system or other dependencies.
- [ ] When manage own's project, prefer a Semantic Version.
