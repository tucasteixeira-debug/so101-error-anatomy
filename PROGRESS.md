# Progress Log

A dated record of the project, newest first. Each entry covers one session or a span of sessions and lists, in plain terms:

- **Achieved**: concrete, verifiable outcomes, quantified where possible.
- **Formation**: the questions worked through, across the full stack the project rests on. That includes computing and operating systems, communication, electronics, mechanics, kinematics, control, measurement and statistics, perception, and machine learning.
- **Not achieved / open**: what didn't work, what is blocked, and what remains.

The project started from zero in most of these areas. The Formation lists record what was studied; they are not a claim of mastery. Entries are drafted with an AI-assisted workflow from private working notes, and each is reviewed by hand before it is committed.

---

### 2026-09-12 · Project planning and development environment setup

**Achieved**
- Semester time budget estimated against course load; single-semester completion kept as a stretch goal.
- Working method set: concepts built one at a time from physical intuition, alongside hands-on work.
- Camera setup revised to two cameras (wrist-mounted and overview); hardware kit sourced.
- Ubuntu 24.04 LTS installed as dual-boot, with NVIDIA GPU drivers for later policy training.
- LeRobot installed with Feetech servo support in a dedicated Python 3.12 environment; import verified.
- Development tooling installed: version control, code editor, Python package manager.

**Formation — questions worked through**
- Where does the boundary between hardware and software lie? (transistors as switches, bits, memory from feedback latches)
- How does a processor execute a stored program? (instruction sets, assembly, fetch–execute cycle)
- What is an operating system kernel, and what role do device drivers play?
- How do programs communicate with peripherals? (device protocols such as Modbus, memory-mapped I/O)
- Why is Linux the prevailing platform for robotics development? (ecosystem, real-time kernel extensions, file-based device access)
- How are Python dependencies isolated per project? (conda environments, interpreter version requirements)

**Not achieved / open**
- First LeRobot install failed: third-party guides specify Python 3.10, while current LeRobot requires 3.12 or newer.
- Measurement method (camera fiducials vs. mechanical fixture) not yet evaluated.
- Task geometry and policy choice not yet fixed.
