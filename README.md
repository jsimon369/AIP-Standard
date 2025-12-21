AIFP — AI First Project Format (.aifp)
Part of the AI First Exchange (AIFX)

AIFP (AI First Project Format) is an open, ZIP-based container standard for complete AI-generated projects. It packages audio, video, images, prompts, scripts, timelines, settings, metadata, licensing, and provenance into a single portable .aifp file designed for transparent, inspectable, and exchangeable AI workflows.

AIFP is the project-level container in the AIFX format family, enabling creators, tools, and platforms to share complex, multi-asset AI productions with clear structure, declared authorship, and long-term interoperability.

🧩 Relationship to AIFX

AIFP is part of the AI First Exchange (AIFX) family of AI-native formats:

AIFM — AI First Music (.aifm)

AIFV — AI First Video (.aifv)

AIFI — AI First Image (.aifi)

AIFP — AI First Project (.aifp)

AIFP is designed to bundle and reference AIFM, AIFV, and AIFI assets within a single project container while preserving provenance, workflow metadata, and verification status.

📚 Overview

An .aifp file represents a complete AI project environment.
It may include:

media assets (audio, video, images)

prompts and narratives

timelines and sequences

AI parameters and toolchains

declared authorship and contributors

licensing and rights documentation

verification and integrity metadata

AIFP prioritizes workflow transparency and reproducibility-oriented documentation, without asserting guarantees beyond the recorded creation process.

📦 AIFP Container Structure

An .aifp file is a ZIP container with a standardized directory layout:

/
  manifest.json                 # REQUIRED: primary project manifest
  assets/
    audio/                      # OPTIONAL
    video/                      # OPTIONAL
    images/                     # OPTIONAL
    models/                     # OPTIONAL (snapshots or references)
  prompts/
    generation.txt              # OPTIONAL: global project prompt
    narrative.txt               # OPTIONAL: script or story text
    settings.json               # OPTIONAL: project-level AI parameters
  timeline/
    sequence.json               # OPTIONAL: scenes, layers, timing
    edits.json                  # OPTIONAL: user or editor changes
  metadata/
    project.json                # OPTIONAL: tags, categories, app data
  legal/
    license.txt                 # OPTIONAL
    terms.txt                   # OPTIONAL
  extra/
    notes.md                    # OPTIONAL: documentation or comments


This structure allows AIFP to represent projects ranging from simple AI outputs to complex, multi-modal productions.

🧠 Key Capabilities
✔ Complete AI Project Packaging

AIFP can contain everything needed to inspect, exchange, and continue an AI project, including:

audio (music, stems, sound design)

video (scenes, renders, clips)

images (concept art, frames, references)

prompts (global and per-scene)

scripts and narratives

timelines and sequences

editor or pipeline metadata

AI parameters and tool references

✔ AI-Native Metadata

AIFP preserves declared AI workflow details such as:

prompt histories

parameter settings

model identifiers or references

seed values (where available)

generation engines and toolchains

processing steps

This metadata supports collaboration, auditing, and archival use cases.

✔ Timeline & Layer Representation

AIFP includes a timeline model capable of representing:

scenes

layers

cuts and transitions

effects

keyframes

multi-modal synchronization

This makes AIFP suitable for AI filmmaking, animation, music-video, and interactive workflows.

✔ Provenance & Authorship Documentation

The project manifest may record:

creator identity (declared)

contributors

AI tools and pipelines

creation timestamps

licensing and rights statements

AIFP records declared provenance and workflow metadata.
It does not assert absolute origin beyond the documented creation process.

✔ Extensible & Tool-Friendly

AIFP is designed to be:

ZIP-based

JSON-driven

easy to parse

architecture-agnostic

forward-compatible

Developers can adapt AIFP for:

music DAWs

video editors

AI animation tools

game engines

XR / VR creation platforms

collaborative AI studios

📑 manifest.json (Simplified Example)
{
  "aifp_version": "1.0.0",
  "id": "aifp-2025-000001",
  "title": "Project Title",
  "creator": "CreatorName",
  "description": "AI-first multi-asset project",
  "ai_generated": true,

  "provenance": {
    "creator_handle": "YourName",
    "creation_utc": "2025-12-06T03:00:00Z",
    "tool_chain": [
      "Suno",
      "Veo",
      "Stable Diffusion",
      "AIFX Converter v1.0"
    ]
  },

  "project": {
    "type": "multimedia",
    "assets": {
      "audio": ["assets/audio/music.wav"],
      "video": ["assets/video/scene01.mp4"],
      "images": ["assets/images/frame01.png"]
    },
    "timeline": "timeline/sequence.json"
  },

  "files": {
    "license": "legal/license.txt",
    "global_prompt": "prompts/generation.txt"
  }
}


Future versions may optionally include:

persona

verification_tier

signature

integrity_hash

🛡️ Verification & Integrity (AIFX-Aligned)

AIFP supports AIFX verification tiers through manifest fields:

Declared Authenticity

Verified Creator

Platform / Pipeline Verified (where supported)

Verification attests to metadata completeness, integrity, and signing status, not facts outside the recorded workflow.

🌐 MIME Type

Proposed MIME type:

application/aifp

🔄 Versioning

AIFP follows semantic versioning:

1.x.x — backward-compatible enhancements

2.x.x — backward-incompatible schema changes

Unknown fields should be safely ignored to maintain compatibility.

🛠 Tooling (Planned)

Planned AIFP utilities:

aifpwrap — package assets + metadata into .aifp

aifp-validate — validate files against the spec

aifp-core — libraries for reading/writing AIFP containers

📬 Contributing

AIFP is an open specification under the AI First Exchange.

Contributions, proposals, and improvements are welcome.

📝 License

This specification is released under the MIT License.
