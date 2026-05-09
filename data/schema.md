# Data Schema

The OpenBOX website reads approved event data from this repository. Bot-generated pull requests should preserve these field names.

## `registrations.json`

The file stores an array of registration objects.

```json
[
  {
    "githubUsername": "octocat",
    "name": "Mona Lisa",
    "introduction": "AI agent builder focused on Web3 automation.",
    "contactMethod": "Telegram: @mona",
    "wantsTeam": "maybe",
    "comment": "Interested in agent workflow projects.",
    "submittedAt": "2026-05-29T08:00:00.000Z"
  }
]
```

## `projects.json`

The file stores an array of project objects.

```json
[
  {
    "id": "agent-workflow-studio",
    "name": "Agent Workflow Studio",
    "track": "AI Agent",
    "summary": "A no-code workflow canvas for coordinating autonomous agents.",
    "team": "Mona Lisa",
    "github": "https://github.com/example/agent-workflow-studio",
    "demo": "https://example.com/demo",
    "pitchDeck": "https://example.com/deck.pdf",
    "members": [
      {
        "githubUsername": "octocat",
        "role": "Builder"
      }
    ],
    "submittedAt": "2026-05-29T10:00:00.000Z"
  }
]
```

## Notes

- Keep `registrations.json` and `projects.json` as valid JSON arrays.
- Use ISO timestamps for `submittedAt`.
- Keep public contact information limited to what participants submit intentionally.
