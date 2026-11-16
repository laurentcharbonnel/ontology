# Enterprise ontology — framing

## What is an enterprise ontology?
An enterprise ontology defines business concepts, their meanings, relationships and constraints independently of any particular database or application. It supports a common language across teams and data domains.

Distinguish:
- **Glossary / terminology:** terms, definitions, synonyms and preferred labels.
- **Taxonomy:** classification and hierarchical organization of concepts.
- **Ontology:** concepts, relations, properties and potentially formal axioms or constraints.
- **Data model:** representation of information for systems and storage.

## Relevant standards and languages
| Standard | Primary contribution |
| --- | --- |
| ISO 704 | Principles and methods for terminology work |
| ISO 1087 | Vocabulary and concepts used in terminology work |
| OMG SBVR | Business vocabulary and business rules |
| W3C SKOS | Concept schemes, preferred/alternative labels and broader/narrower relationships |
| W3C RDF | Graph-based representation of statements |
| W3C RDFS / OWL | Schema and formal ontology semantics |

These are complementary rather than interchangeable. Selection depends on requirements for interoperability, inference, governance and tooling.

## Proposed knowledge-capture workflow
1. **Define scope:** business domain, stakeholders, use cases and competency questions.
2. **Capture knowledge:** interview domain experts and inspect existing glossaries, business rules, data contracts and schemas.
3. **Normalize terminology:** identify concepts, definitions, synonyms, homonyms and naming conflicts.
4. **Model concepts:** define identities, relationships, classifications, constraints and examples.
5. **Validate:** review real scenarios and counterexamples with business owners.
6. **Publish and govern:** version concepts, assign ownership and manage changes.
7. **Connect to implementations:** trace concepts to conceptual, logical and physical models, APIs and data products.

## Example
For a financial information domain, concepts might include **Company**, **Reporting Period** and **Fiscal Calendar**. A reporting period can be defined relative to a company's fiscal calendar; it should not be modeled merely as a string field.

## Open considerations
- Which business questions must the ontology answer?
- What level of formality is justified: glossary/SKOS, business rules/SBVR, or OWL?
- Who approves definitions and cross-domain mappings?
- How are versions and changes propagated to downstream systems?
