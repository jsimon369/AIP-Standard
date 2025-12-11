# COPYRIGHT & HUMAN AUTHORSHIP GUIDANCE (AIP Standard)

The AI Format Foundation recognizes that copyright protection for AI-assisted works requires meaningful human creative contribution. The AIP Standard supports documentation of human authorship in complex, multi-asset AI projects through structured metadata, provenance, and workflow history.

## 1. Human Authorship Requirements

An AI-assisted project may qualify for copyright if a human:
- Designs the overall concept, story, or creative direction  
- Writes prompts, scripts, instructions, or scene breakdowns  
- Chooses, arranges, or sequences AI-generated media  
- Edits or refines assets such as audio, video, images, or text  
- Makes expressive decisions that shape the final project  

Purely autonomous assembly or generation without human creative involvement is not copyrightable.

## 2. How AIP Supports Copyright Claims

AIP metadata captures:
- Creator identity (name, handle, email)  
- Human-authored prompts, scripts, and notes  
- Timeline and sequence metadata  
- Editing steps for each asset  
- Provenance of imported files (audio, video, image, text, models)  
- Timestamps and toolchain history  

AIP can serve as a comprehensive record of the human creative process across an entire project.

## 3. Recommended Manifest Fields for Legal Compliance

Creators may include these optional fields:

"human_authorship_statement": "I affirm that I contributed creative authorship...",
"human_signature": "Name or digital signature hash",
"creator_email": "email@example.com",
"editorial_notes": "Summary of human creative decisions."


## 4. Ownership

Copyright belongs to the human author(s) who contributed meaningful creative decisions within the project.  
Unedited or uncurated AI output does not qualify for copyright protection on its own.

## 5. Licensing

Creators may include licensing details in `legal/license.txt`, `license.json`, or similar files.  
AIP users are responsible for complying with all applicable laws and content licenses.
