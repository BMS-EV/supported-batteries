# Supported EV Batteries

Public database of **70 battery/BMS profiles** supported by [BMS-EV](https://bms-ev.com/) controllers for reuse as home stationary energy storage.

**Full documentation:** [docs.bms-ev.com/batteries/](https://docs.bms-ev.com/batteries/)  
**Interactive matrix:** [docs.bms-ev.com/compatibility/](https://docs.bms-ev.com/compatibility/)

## Data

- [batteries.csv](batteries.csv) — machine-readable list of all 70 supported profiles (65 OEM EV pack profiles + 5 DIY/stationary BMS profiles), with the count of compatible inverters per profile

## By manufacturer

| Manufacturer | Models | Documentation |
|-------------|--------|---------------|
| Tesla | Model 3, Model Y, Model S, Model X (60-100 kWh) | [Tesla batteries](https://docs.bms-ev.com/batteries/tesla-model-3/) |
| BMW | i3 (60/94/120 Ah), iX/i4 platform, PHEV | [BMW i3](https://docs.bms-ev.com/batteries/bmw-i3/) |
| Nissan | Leaf 24/30/40/62 kWh, Ariya, e-NV200, Sakura | [Nissan Leaf](https://docs.bms-ev.com/batteries/nissan-leaf/) |
| Volkswagen (MEB) | ID.3, ID.4, ID.5, Skoda Enyaq, Audi Q4 e-tron, Cupra Born, Ford Explorer EV | [VW MEB](https://docs.bms-ev.com/batteries/vw-meb/) |
| Hyundai/Kia (E-GMP) | Ioniq 5/6, EV6, EV9, Kona 39/64 kWh, e-Niro | [Hyundai/Kia E-GMP](https://docs.bms-ev.com/batteries/hyundai-kia-egmp/) |
| Renault | Zoe Gen1/Gen2, Twizy, K-ZE, Kangoo, Fluence | [Renault Zoe](https://docs.bms-ev.com/batteries/renault-zoe/) |
| Stellantis (CMP/e-CMP) | Peugeot e-208/2008, Citroen e-C4/e-C3, Opel Corsa-e/Mokka-e, Fiat, Toyota Proace Electric | [Stellantis CMP](https://docs.bms-ev.com/batteries/stellantis-cmp/) |
| BYD | Atto 3, Seal, Seal U, Song Plus, Dolphin mini | [BYD Atto 3](https://docs.bms-ev.com/batteries/byd-atto-3/) |
| MG | MG4, MG5, MG Marvel R, ZS EV, HS PHEV | [MG 4](https://docs.bms-ev.com/batteries/mg-4/) |
| Ford | E-Transit, Mustang Mach-E | [Ford Mach-E](https://docs.bms-ev.com/batteries/ford-mustang-mach-e/) |
| Volvo/Polestar | EX30, XC40/C40, Polestar 2 | [docs.bms-ev.com/batteries/](https://docs.bms-ev.com/batteries/) |
| Other | Chevrolet Bolt, Rivian R1T, Mitsubishi i-Miev, Jaguar I-PACE, Porsche Taycan, Audi e-tron GT, Mini Cooper Electric, Dacia Spring | [All batteries](https://docs.bms-ev.com/batteries/) |

## Compatibility Matrix

Full **70 battery/BMS profiles × 56 inverter variants** matrix (3,768 pairs): https://docs.bms-ev.com/compatibility/

Machine-readable: [supported-inverters](https://github.com/BMS-EV/supported-inverters) · [full compatibility CSV](https://github.com/BMS-EV/bms-ev-docs/blob/main/compatibility.csv)

## How to contribute

Missing a battery? Have you successfully installed one that isn't listed? [Open an issue](https://github.com/BMS-EV/supported-batteries/issues) with details.

## License

[MIT License](LICENSE)

## Contact

- Shop: https://bms-ev.com/
- Documentation: https://docs.bms-ev.com/
- Email: office@bms-ev.com

## Counting basis

The 70 figure counts firmware profiles, not OEM EV pack variants alone: 65 OEM EV pack profiles plus 5 DIY/stationary BMS profiles (Orion, RJXZS, SimpBMS, FoxESS HV2600, Pylon HV). The `profile_type` column in [batteries.csv](batteries.csv) distinguishes them.

**Correction, 2026-09-19.** Earlier versions published 73 profiles. Three entries were naming duplicates of existing profiles (Citroen Spacetourer EV, MG ZS EV, Toyota Proace EV), introduced by the WooCommerce catalogue export where one product can appear under more than one category. They were removed; their full profiles remain under the canonical names.
