# self-improving-skills

An agent skill that makes your other skills get better every time you use them.

AI coding agents forget everything between sessions. The only thing that lasts is what is written into skill files and memory. This skill is the loop that does that writing for you:

1. **Ask** for feedback after each finished task.
2. **Sort** each lesson: how-to goes into the skill, personal taste goes into memory, the rest is dropped.
3. **Write** it as one short, concrete line. No bloat.
4. **Find gaps**: search online for existing skills that would help ([skills.sh](https://skills.sh), `find-skills`, web search).
5. **Ask before installing**: explain what it does, the risk and the cost, then install only on a yes.
6. **Start new skills** when a new kind of task has none.

It came out of real work: making YouTube Shorts with Claude Code and Remotion. After a few videos the video skill knew what the viewer liked, which tools cost too much, and which bugs to avoid, because this loop wrote it down each time.

## Install

With the [skills CLI](https://github.com/vercel-labs/skills) (Claude Code, Codex, Cursor, Copilot and more):

```bash
npx skills add https://github.com/Hakkixxx/self-improving-skills --skill self-improving-skills -g
```

Or by hand: copy `skills/self-improving-skills/` into `~/.claude/skills/` (global) or `<project>/.claude/skills/` (one project).

Recommended: also install `find-skills` so step 4 can search skills.sh.

```bash
npx skills add https://github.com/vercel-labs/skills --skill find-skills -g
```

## Use

Nothing to call. The agent runs it after a task made with a skill is done. You can also say "run the improve loop" or "update the skill with what we learned".

## Safety

The skill never installs anything without asking you. Third-party skills run with your agent's full permissions, so read what you install.

---

## Türkçe

Diğer skill'lerini her kullanımda daha iyi yapan bir skill.

Yapay zekâ ajanları oturumlar arasında her şeyi unutur. Kalıcı olan tek şey skill dosyalarına ve hafızaya yazılandır. Bu skill o yazma işini senin yerine yapar: iş bitince geri bildirim ister, dersi doğru yere yazar, eksik bir yetenek varsa internetten hazır skill arar ve kurmadan önce sana ne işe yaradığını, riskini ve ücretini söyleyip izin ister.

Kurulum için yukarıdaki `npx skills add` komutunu kullan.

## Author

Hakkı Kaan Yeşil ([@Hakkixxx](https://github.com/Hakkixxx))

## License

MIT
