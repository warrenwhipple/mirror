# Scaffolding a new MIRROR.md

Read this file only after the user has explicitly agreed to scaffold a new mirror.

The prime directive still applies during scaffolding: the mirror only works if every word of content in it is the human's. Your job here is to place a blank template and hand over ownership — not to fill it in, not even helpfully.

## Steps

1. **Confirm filename and location.** Default is `MIRROR.md` at the repository root. If the user wants a scoped mirror (for example, one per subproject), use `MIRROR-<scope>.md` at the root. If a file with the target name already exists, stop and tell the user — never overwrite.

2. **Copy the template verbatim.** Copy `assets/MIRROR.template.md` from this skill directory to the target path, byte-for-byte:

   ```
   cp <skill-dir>/assets/MIRROR.template.md <repo-root>/MIRROR.md
   ```

   Do not customize it, do not replace the placeholder bullets with inferred project content, and do not pre-fill Goals or Next based on what you know about the project. Pre-filled content is agent words wearing the human's byline, and it poisons the file from day one. The template intentionally ships with its own embedded Agent Rules section, so agents encountering the file without this skill installed still behave correctly.

3. **Hand over ownership.** Tell the user the file is created and is now entirely theirs. Suggest they start by rewriting the placeholder bullets under **Goals** and **Next** in their own words — those two sections carry most of the orientation value — and that the intro paragraph and Agent Rules are theirs to keep or reword as they like. Keep this handoff to a few sentences.

4. **Stop.** Do not offer to draft content for any section, do not interview them to generate content, and do not open the file again unless asked to check it.

If the user dictates content and asks you to type it into the file for them, decline per the hard rules in SKILL.md — even transcription establishes the habit of agent hands in the file. They should edit it directly; it is deliberately short.
