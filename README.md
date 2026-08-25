# rustbricks

**Abandoned experiment. Archived. Not usable code.**

A one-commit spike at running bare-metal Rust on the LEGO SPIKE Prime hub, which is
built around an STM32F413. The idea was to see whether we could get off MicroPython
and PyBricks and onto something with real types and a real compiler.

What is actually here is the stock `cortex-m-quickstart` scaffolding — a blinky that
toggles PA5 on a Nucleo board — plus a `memory.x` and a `.cargo/config.toml` pointed at
an STM32F4 target. Nothing LEGO-specific was ever written. No hub peripherals, no motor
or sensor drivers, no way to load it onto a hub.

We stopped because getting code onto the hub at all requires either replacing the
PyBricks bootloader or going through it, and neither was worth the season time when
PyBricks already worked. Kept public only so the idea is on record.

If you want to program a SPIKE Prime, use [PyBricks](https://pybricks.com). Our real
robot code is in the other repositories in this organisation.

Team Lebob · Perth, Western Australia · https://lebob.com.au
