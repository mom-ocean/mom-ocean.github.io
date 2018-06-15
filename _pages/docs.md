---
layout: home
permalink: /docs/
author_profile: true
toc: true
sidebar:
    nav: "quicklinks"
---
## Documentation
#Technical Documents

                each doc in web_docs
                    li
                        a(href="#{doc.url}") #{doc.name}
                each doc in test_case_docs
                    li <a href="docs/project/#{doc.filename}")>#{doc.name}</a> [PDF]

            h2 #{project} Foundations and History

            p The following documents provide a description of the physical, mathematical, numerical, and computational foundations for the various versions of MOM. There is also a document that gives a detailed account of MOM history. They are provided here partly for their historical relevance, as well as for their pedagogical value.

            ul
                each doc in manual_docs
                    li <a href="docs/project/#{doc.filename}")>#{doc.name}</a> [PDF]

            h2 Contributing to #{project}

            p These documents explain how to contribute code, configuration or documentation changes to #{project}.

            ul
                each doc in other_docs
                    li
                        a(href="#{doc.url}") #{doc.name}


            h2 Documentation Development

            p The documentation for #{project} is just as important as the code itself. Where feasible, the source of all documentation is developed alongside the code within the main repository. This allows developers to keep it up to date as part of their regular work flow.

            p If you find something incomplete, incorrect or incomprehensible, please report this as an issue on the <a href="https://github.com/BreakawayLabs/mom/issues">task tracker</a>.