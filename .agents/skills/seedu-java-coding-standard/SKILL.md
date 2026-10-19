---
name: seedu-java-coding-standard
description: Apply the SE-EDU basic and intermediate Java conventions when writing, modifying, or reviewing Java production code and tests in this project.
---

# SE-EDU Java coding standard

Before changing Java, read the [basic and intermediate standard](https://se-education.org/guides/conventions/java/intermediate.html). It is the normative reference; this checklist is not a replacement. Consult its linked Google Java guide for uncovered topics. Do not import the advanced-only SE-EDU rules.

## Review checklist

- Use English names: lowercase packages, PascalCase noun types, camelCase variables and verb methods, uppercase underscore-separated constants. Treat acronyms as words; make booleans read as predicates, collections plural, and related constants share prefixes. Test names may separate feature, scenario, and outcome with underscores.
- Indent with four spaces and continuations with eight extra spaces. Aim below 110 columns; never exceed 120. Use K&R braces, readable operator spacing, and blank lines between logical groups. Wrap after commas and before operators.
- Package every class; order explicit imports consistently. Attach array brackets to types. Initialize variables in the smallest feasible scope. Encapsulate fields except constants and behaviorless data classes.
- Always brace loops and conditionals; put their bodies on separate lines. Mark intentional switch fallthrough.
- Write American-English comments. Document classes and public methods, except tests, accessors, and exact overrides. Use concise third-person Javadoc summaries, aligned asterisks, separated tags, and punctuated parameter descriptions. Document all parameters or none when self-explanatory.

## Repository workflow

Apply this standard to all Java source, including test helpers. Follow `config/checkstyle/checkstyle.xml` for this repository's import grouping. Inspect that configuration and `suppressions.xml` before relying on automated coverage.

Review naming, scope, encapsulation, and documentation manually as well: passing Checkstyle alone does not establish full compliance. Preserve behavior when correcting style; update callers and tests if encapsulation changes an internal API. Preserve stored data formats and user-facing command syntax.

Run `./gradlew checkstyleMain checkstyleTest` after Java edits, and the relevant tests when changes affect executable code. For a project-wide migration, run `./gradlew checkstyleMain checkstyleTest test`. Report any checks that cannot run. Do not weaken checks or add suppressions merely to hide violations.
