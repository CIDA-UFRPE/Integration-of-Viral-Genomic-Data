# G2G Matcher: Viral Genomic Data Integration Tool 
G2G Matcher is a Python-based framework designed to resolve data fragmentation and redundancy between GenBank and GISAID genomic repositories. By employing a hierarchical five-stage pipeline, the tool identifies duplicate biological samples that are often "double-counted" due to inconsistent metadata or identifiers.  

## Key Features:
- Hierarchical Matching: Combines exact FASTA identity, Fuzzy string matching (Levenshtein distance) for isolates, and LCDL (Location, Date, Length) metadata reconciliation.  
- NLP-Powered Preprocessing: Uses custom Regex to standardize and extract isolate identifiers from unstructured GenBank titles.
- Phylogenetic Quality Control: Automatically filters out experimental artifacts, vaccine-derived strains, and laboratory-adapted lineages to ensure biological relevance.
- Conflict Resolution: Assigns high-confidence integration statuses (MATCH, POTENTIAL, UNIQUE) to facilitate automated or expert-guided curation.
