# VOID TETHER — 1968 Spacewalk Duel

A zero-g spacewalk action and tether grappling arcade game inspired by 1960s vintage sci-fi pulp space artwork. Built specifically for **[webcade.fun/arcade](https://webcade.fun/arcade)** and mobile browsers.

Live Shareable URL: **[https://21e8-miner.github.io/void-tether/](https://21e8-miner.github.io/void-tether/)**

---

## Game Overview

Step into the boots of a 1968 spacewalker drifting in the deep obsidian void. Harpoon derelict satellites, swing using centrifugal momentum, cut enemy life-support lines, and manage your triple yellow oxygen tanks before life support fails.

### Features
- **Zero-G Physics**: Inertial drift, RCS gas thruster mechanics, and realistic tether physics.
- **Tether Harpoon**: Sling around satellites and derelicts, or grapple enemy cosmonauts.
- **Sabotage & Combat**: Slice lifelines with the tether cutter or fire raygun bolts.
- **Oxygen Life Support**: Yellow triple tanks deplete with thruster burns; harvest floating canisters to survive.
- **Webcade Arcade Integration**: Native `postMessage` protocol for host iframe score tracking and cabinet controls.

---

## Controls

### Mobile Touch Controls
- **Left Thumb Drag**: 360° RCS flight vector thruster
- **◎ Tether Button**: Harpoon nearest satellite / reel in / slingshot
- **⚡ Laser Button**: Fire raygun dart bolt
- **✂ Cut Button**: Slice active tether or enemy life-support lines
- **II Button**: Pause / Resume

---

## Webcade Integration

```javascript
window.addEventListener("message", (e) => {
  if (e.data && e.data.voidTether) {
    console.log("Webcade Event:", e.data.voidTether, e.data);
  }
});
```

---

## License
MIT License.
