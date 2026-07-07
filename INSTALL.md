# Install Competitor Language X-Ray

The same skill folder works for Codex and Claude Code. Claude Desktop/Cowork-style apps can use the packaged `.skill` bundle when supported.

## Codex

Copy the skill folder into your Codex skills directory:

```powershell
Copy-Item -Recurse -Force ".\competitor-language-x-ray" "$env:USERPROFILE\.codex\skills\competitor-language-x-ray"
```

Then start a new Codex thread and ask:

```text
Use $competitor-language-x-ray to research these ecommerce competitors: ...
```

You can also install it project-locally by copying the folder into:

```text
.codex/skills/competitor-language-x-ray
```

## Claude Code

Copy the same folder into Claude's skills directory:

```bash
cp -R competitor-language-x-ray ~/.claude/skills/competitor-language-x-ray
```

Optional command shortcut:

```bash
cp commands/x-ray.md ~/.claude/commands/x-ray.md
```

Then use:

```text
/x-ray brand1.com brand2.com "category: dog water fountains" "ICP: anxious pet owners"
```

## Claude Desktop / Cowork-Style Skill Bundle

Use the packaged file:

```text
competitor-language-x-ray.skill
```

Open or import it in the app if your Claude surface supports saved skills.

## Rebuild The Skill Bundle

From this repo root:

```powershell
Compress-Archive -Path ".\competitor-language-x-ray" -DestinationPath ".\competitor-language-x-ray.zip" -Force
Copy-Item ".\competitor-language-x-ray.zip" ".\competitor-language-x-ray.skill" -Force
Remove-Item ".\competitor-language-x-ray.zip"
```