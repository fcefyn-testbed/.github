# FCEFYN Testbed

HIL lab for OpenWrt and LibreMesh at [FCEFyN](https://fcefyn.unc.edu.ar/) - [UNC](https://www.unc.edu.ar/), Córdoba, Argentina.

Real routers on a rack, orchestrated with [Labgrid](https://labgrid.readthedocs.io/), tests with [pytest](https://docs.pytest.org/). Single-node runs on hardware or QEMU, multi-node mesh, ZeroTier for remote dev when you need it.

<p align="center">
  <img src="https://github.com/user-attachments/assets/ce9675ef-54e8-4972-9a40-b96d34cb2ddb" alt="rack" width="280" />
  &nbsp;
  <img src="https://github.com/user-attachments/assets/82dcb675-6f7f-4b4a-9d8d-9e6b85cf965f" alt="rack drawer: Arduino, relays, adapters" width="420" />
</p>

## Rack (current)

| Device | Role | CI / tests |
|--------|------|------------|
| Belkin RT3200 #1 | DUT | yes |
| Belkin RT3200 #2 | DUT | yes |
| Belkin RT3200 #3 | DUT | yes |
| Banana Pi BPI-R4 | DUT | yes (wired mesh; WiFi kmods excluded on 24.10) |
| OpenWrt One | DUT | yes |
| LibreRouter #1 | DUT | yes |
| LibreRouter #2, #3 | mounted, reserved | not yet |
| TP-Link TL-WDR3500 | testbed gateway (VLAN trunk) | n/a |

Full port map, serial symlinks, SSH: [rack cheatsheet](https://fcefyn-testbed.github.io/fcefyn_testbed_utils/operar/rack-cheatsheets/) · [DUT config](https://fcefyn-testbed.github.io/fcefyn_testbed_utils/configuracion/duts-config/)

## Repos

| Repo | What |
|------|------|
| [fcefyn_testbed_utils](https://github.com/fcefyn-testbed/fcefyn_testbed_utils) | Ansible, scripts, switch/relay control, docs site |
| [libremesh-tests](https://github.com/fcefyn-testbed/libremesh-tests) | pytest suite + Labgrid targets (fork of [openwrt-tests](https://github.com/aparcar/openwrt-tests), mesh support) |
| [lime-packages](https://github.com/fcefyn-testbed/lime-packages) | LibreMesh fork, firmware build + CI |

## Links

| | |
|---|---|
| Docs | [fcefyn-testbed.github.io/fcefyn_testbed_utils](https://fcefyn-testbed.github.io/fcefyn_testbed_utils/) |
| CI dashboard | [ci-results/dashboard](https://fcefyn-testbed.github.io/fcefyn_testbed_utils/ci-results/dashboard.html) |
| Grafana | [fcefyn-testbed.duckdns.org](https://fcefyn-testbed.duckdns.org/) (invite only; [how it works](https://fcefyn-testbed.github.io/fcefyn_testbed_utils/configuracion/grafana-public-access/)) |

## Hardware sponsors

OpenWrt One and BPi-R4 ([Banana Pi](https://banana-pi.org/)), LibreRouter ([AlterMundi](https://altermundi.net/)), Belkin RT3200 + host laptop ([INTI](https://www.argentina.gob.ar/inti)). Details: [hardware catalog](https://fcefyn-testbed.github.io/fcefyn_testbed_utils/configuracion/catalogo-hardware/).

## Upstream

[openwrt-tests](https://github.com/aparcar/openwrt-tests), [LibreMesh](https://libremesh.org/), [OpenWrt](https://openwrt.org/).

## Contact

Open an issue in [fcefyn_testbed_utils](https://github.com/fcefyn-testbed/fcefyn_testbed_utils/issues).
