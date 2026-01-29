# Unity + Cursor Rules (Beginner-safe)

## Tech stack
- Unity: LTS (I’m a beginner; prefer simple solutions)
- Language: C#
- Target: 2D mobile game (portrait)

## Project structure
- All scripts go under: `Assets/_Project/Scripts/...`
- Scenes go under: `Assets/_Project/Scenes/`
- Prefabs go under: `Assets/_Project/Prefabs/`
- UI assets go under: `Assets/_Project/UI/`
- Art assets go under: `Assets/_Project/Art/`

## Coding standards
- Keep scripts short and readable.
- Prefer Inspector references (serialized fields) over `FindObjectOfType` / `GameObject.Find`.
- Avoid heavy code in `Update()`; use events/coroutines/timers when possible.
- Add clear comments for beginners.
- Use clear names and consistent formatting.
- When creating new code: state exactly where to place files (full path).

## Unity behavior rules
- Use `MonoBehaviour` for runtime behavior.
- Use `ScriptableObject` only when it truly helps (configs/data).
- For saving simple data: `PlayerPrefs` is OK.
- Avoid singletons unless there’s a clear reason; prefer a `GameRoot` object per scene.

## Dependencies / packages
- Don’t require external packages unless I explicitly say so.
- Don’t assume TextMeshPro, Input System, URP, Addressables, etc. unless I confirm.
- If a feature would be better with a package, suggest it as an option, but also provide a version that works without it.

## Output format I want from Cursor
- Step-by-step instructions.
- Full code blocks (copy/paste ready).
- Tell me what GameObject(s) to create and what scripts to attach.
- Tell me what to click in Unity (menus, settings).
- Include a simple test procedure (what I should see in Console/UI when I press Play).
