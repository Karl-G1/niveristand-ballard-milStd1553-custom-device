# Ballard MIL-STD-1553 Custom Device

The **Ballard MIL-STD-1553 Custom Device** allows use of [Astronics MIL-STD-1553 PXIe Modules with Ballard Technology](https://www.ni.com/en-us/shop/hardware/products/pxi-mil-std-1553-interface-module.html) in VeriStand. The custom device targets one **core** of a Ballard MIL-STD-1553 PXIe module. To target multiple modules or multiple cores on the same module, use multiple instances of this custom device.

The custom device supports the following functionality:
- Import configuration files via scripting and System Explorer
- LabVIEW scripting of the custom device configuration
- Viewing read-only configuration in System Explorer
- Transmit and Receive configured messages, command words, and status words
   - Scheduled and Acyclic
   - Multiple parameters per message
   - Multiple messages on one or both channels per core

## Requirements

- PXI Linux RT Controller
- Supported Ballard MIL-STD-1553 PXI Module

**Note**: Only NI-keyed PXI modules are supported by the custom device. The part number should have the form `LV-222-###-###`, where `###` stands for the core configuration. **550** and **555** core models are supported. See the mapping between NI and Ballard part numbers on [ni.com](https://www.ni.com/en-us/support/documentation/supplemental/17/astronics-ballard-and-national-instruments-part-number-mapping.html).

## Getting Started Documentation

- [User Guide](Docs/User%20Guide/User%20Guide.md)
- [Parameters XML File Schema](Docs/Parameters%20XML%20File/Parameters%20XML%20File.md)

## LabVIEW Source Code Version

LabVIEW 2020

## Dependencies

### Running the custom device

- [VeriStand 2020 or later](https://www.ni.com/ro-ro/support/downloads/software-products/download.veristand.html#382072)
- Optional: [Astronics Ballard Avionics Driver](https://www.ni.com/en-us/support/downloads/drivers/download.astronics-ballard-avionics-driver.html#370805)

### Developing or building from source

- [VeriStand Custom Device Development Tools](https://github.com/ni/niveristand-custom-device-development-tools)
- [NI VeriStand Custom Device Message Library](https://github.com/ni/niveristand-custom-device-message-library)
- [NI VeriStand Custom Device Testing Tools](https://github.com/ni/niveristand-custom-device-testing-tools)
- [Astronics Ballard Avionics Driver and LabVIEW API](https://www.ni.com/en-us/support/downloads/drivers/download.astronics-ballard-avionics-driver.html#370805)

## Git History & Rebasing Policy

Branch rebasing and other history modifications will be listed here, with several notable exceptions:
- Branches prefixed with `dev/` may be rebased, overwritten, or deleted at any time.
- Pull requests may be squashed on merge.

## License

This Ballard MIL-STD-1553 custom device is licensed under an MIT-style license (see LICENSE). Other incorporated projects may be licensed under different licenses. All licenses allow for non-commercial and commercial use.
