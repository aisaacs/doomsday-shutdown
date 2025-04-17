# 💀 doomsday-shutdown

> A Node.js utility for when your program messes up so hard, it deserves the End Times.

**doomsday-shutdown** gives you multiple creative and dangerous ways to shut down, crash, panic, or otherwise obliterate your system. This is not a joke. (Okay, it is. But also it isn't.)

---

## ⚠️ ABSOLUTE WARNING

This library will:
- Shut down your computer
- Crash your OS
- Eat all your RAM
- Forkbomb your CPU

Use only on machines you fully control. **Don't run this in production. Don't run this in staging. Don't run this near your mom.**

---

## 💾 Installation

```bash
npm install doomsday-shutdown
```

---

## 🧨 API

```js
const doom = require('doomsday-shutdown');
```

### `doom.gentleGoodnight()`
> Politely powers down the system.

- ✅ Cross-platform
- 🪟 Windows: uses `shutdown /s /t 0`
- 🐧 Linux/macOS: uses `shutdown -h now`

---

### `doom.yeetThePlug()`
> Forcibly powers off Linux using `/proc/sysrq-trigger`.

- ⚡ Instant power cut.
- 🧯 Risk of filesystem corruption.
- 🔐 Requires root.

---

### `doom.blueScreenOfBoom()`
> Windows force shutdown. Want a real BSOD? You’ll need a native NT call.

- 💥 Calls `shutdown /s /f /t 0`
- 🪦 Good enough for most mortals.

---

### `doom.summonTheKernelDemon()`
> Triggers a Linux **kernel panic**.

- 👹 `echo c > /proc/sysrq-trigger`
- 💣 Unrecoverable system crash
- 🔐 Root access required

---

### `doom.forkocalypse()`
> Forks processes infinitely.

- 🌀 Kills your CPU
- 🧠 You were warned.

---

### `doom.eatTheRAM()`
> Allocates memory forever until you're OOM-killed.

- 🫠 Works on any OS
- 🧽 Your swap file is crying

---

## 🧪 Example

```js
const doom = require('doomsday-shutdown');

// doom.gentleGoodnight();
// doom.yeetThePlug();
// doom.blueScreenOfBoom();
// doom.summonTheKernelDemon();
// doom.forkocalypse();
// doom.eatTheRAM();
```

---

## 👨‍💻 Author

**Alessandro Isaacs**  
Shutdown philosopher. Memory nihilist. Kernel necromancer.

---

## 🧛 License

MIT. But if you misuse this, the ghost of your kernel might haunt you.

---

## 🧟‍♀️ Related Projects

- `fork-bomb-as-a-service`
- `ragequit.sh`
- `reboot-and-cry`
