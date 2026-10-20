# legalize-ie

Ireland legislation in Markdown, version-controlled as a git repository.

Each law is a file; each reform is a commit dated to the real official publication date. The `git log` of any law shows its full history — when it was enacted, which articles changed and by which norm.

Acts published in the eISB annual indexes from 1922 onward, including public Acts, private Acts and constitutional amendments; the current Constitution of Ireland; and the statutory instruments referenced by their amendment histories. This is not a complete collection of statutory instruments or pre-1922 legislation.

## What's inside

- **Acts** (`IE-{year}-act-{number}`) — Public Acts, private Acts (P prefix) and constitutional amendment Acts (C prefix), with distinct identities.
- **Constitution of Ireland** (`IE-1937-constitution`) — The latest consolidated official text, explicitly marked current.
- **Statutory instruments** (`IE-{year}-si-{number}`) — Source instruments needed to resolve amendment histories, including their dependencies.

## Data source

- **Electronic Irish Statute Book — Office of the Attorney General; Law Reform Commission**
  - Enacted legislation and effects: https://www.irishstatutebook.ie
  - Supplementary parliamentary metadata: https://api.oireachtas.ie/v1/legislation
  - Revised Acts and archives: https://revisedacts.lawreform.ie/revacts/chron

## Attribution

> Contains Irish Public Sector Information from the Houses of the Oireachtas, the electronic Irish Statute Book (Office of the Attorney General) and the Law Reform Commission. Copyright remains with the respective licensors. Reused under the [Oireachtas (Open Data) PSI Licence](https://www.oireachtas.ie/en/open-data/license/), incorporating [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/). Sources: https://www.irishstatutebook.ie and https://revisedacts.lawreform.ie.

## Text and history

Enacted texts are marked `as_enacted`. LRC archived PDF snapshots retain their stated cutoff and source URL. Mutable consolidated texts are marked `current`; the notice explains that they cannot establish the text at an earlier commit date.

Amendment records cite the actual amending instrument. Snapshot cutoffs and commencement dates are not represented as new publication dates. Undated source publications omit `Source-Date`. The original publication date remains unchanged across versions.

A verified incomplete source carries a `source_warning` and a visible notice naming the missing provision. The available official text is preserved without reconstruction. Content-bearing binary figures are marked `[image omitted]`; source image counts are retained in metadata.

Paths follow the sharded template declared in `.legalize.yml`. The corpus conforms to the Legalize v0.4 identifier, source, date and history conventions.

## Source terms

eISB and LRC Revised Acts are reused under the Oireachtas (Open Data) PSI Licence, incorporating CC BY 4.0. The LRC confirmed the application of these terms to Revised Acts on 8 October 2026. See the [copyright and re-use policy](https://www.oireachtas.ie/en/copyright-and-reuse/).

Legalize converts source documents into Markdown and structured version history. Formatting and image omissions are described above; LRC editorial annotations, commentary and logos are excluded. Source links, revision cutoffs and source warnings are preserved. This is not the official text of an Act or an official restatement. Legalize is independent and is not endorsed by the source bodies.

The Houses of the Oireachtas disclaim liability arising from reuse and do not certify that the material is current or error-free. Publication does not establish that a provision is in force. Consult the linked official sources and their notices before relying on the text.

## Other countries

This repository is part of **Legalize**, which maintains the legislation of multiple countries as git repos. See https://legalize.dev for the full catalog.

## Support

Legalize is free and open. If this work is useful to you, you can help sustain its hosting and development: [Support this project](https://buymeacoffee.com/legalizedev).

## License

- **Pipeline code**: MIT (https://github.com/legalize-dev/legalize-pipeline)
- **Data**: Oireachtas (Open Data) PSI Licence, incorporating Creative Commons Attribution 4.0 International (CC BY 4.0): https://www.oireachtas.ie/en/open-data/license/. eISB publishes these terms at https://www.irishstatutebook.ie/open-data.html; the Law Reform Commission confirmed their application to Revised Acts on 8 October 2026.
