# FCEFYN Testbed

**Hardware-in-the-loop testing infrastructure for OpenWrt and LibreMesh**

Built at [Facultad de Ciencias Exactas, Físicas y Naturales](https://fcefyn.unc.edu.ar/) - [Universidad Nacional de Córdoba](https://www.unc.edu.ar/) - Argentina.

---

## What is this?

A physical testbed for automated firmware validation on real router hardware. The lab runs continuous integration tests on OpenWrt and LibreMesh firmware using [Labgrid](https://labgrid.readthedocs.io/) for device orchestration and [pytest](https://docs.pytest.org/) for test execution.

The infrastructure supports:

- **Single-node tests** — one device at a time (physical or QEMU)
- **Multi-node mesh tests** — multiple routers forming a mesh network
- **Remote access** — devices reachable via ZeroTier for development and debugging

---

## Repositories

| Repository | Description |
|------------|-------------|
| [**fcefyn_testbed_utils**](https://github.com/fcefyn-testbed/fcefyn_testbed_utils) | Lab infrastructure: Ansible roles, scripts, switch/relay control, documentation |
| [**libremesh-tests**](https://github.com/fcefyn-testbed/libremesh-tests) | Fork of [openwrt-tests](https://github.com/aparcar/openwrt-tests) with LibreMesh multi-node support |

---

## Resources

| Resource | Link |
|----------|------|
| Documentation | [fcefyn-testbed.github.io/fcefyn_testbed_utils](https://fcefyn-testbed.github.io/fcefyn_testbed_utils/) |
| Live Metrics (Grafana) | [fcefyn-testbed.github.io/fcefyn_testbed_utils/configuracion/grafana-publico](https://fcefyn-testbed.github.io/fcefyn_testbed_utils/configuracion/grafana-publico/) |

---

## Hardware

The testbed includes devices donated by the community:

- **OpenWrt One** and **Banana Pi R4** — [Banana Pi](https://banana-pi.org/)
- **LibreRouter** units — [AlterMundi](https://altermundi.net/)
- **Belkin RT3200** routers and host laptop — [INTI](https://www.argentina.gob.ar/inti)

See the [hardware catalog](https://fcefyn-testbed.github.io/fcefyn_testbed_utils/configuracion/catalogo-hardware/) for full details.

---

## Related Projects

- [openwrt-tests](https://github.com/aparcar/openwrt-tests) — upstream single-node testing framework
- [LibreMesh](https://libremesh.org/) — community mesh firmware
- [OpenWrt](https://openwrt.org/) — base firmware

---

## Contact

For questions about the testbed or collaboration inquiries, open an issue in [fcefyn_testbed_utils](https://github.com/fcefyn-testbed/fcefyn_testbed_utils/issues).
