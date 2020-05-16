# vga-text-mode

Verilog code for [VGA-compatible text mode](https://en.wikipedia.org/wiki/VGA-compatible_text_mode) on an [FPGA](https://simple.wikipedia.org/wiki/Field-programmable_gate_array).

## Usage

1. Take files from `src/` and add them to your own project. If you use [hdlmake](https://hdlmake.readthedocs.io/en/master/), you can add this repository itself as a remote module.
1. Other helpful modules are also available in this GitHub organization.
1. Consult the usage example in [hdmi-demo](https://github.com/hdl-util/hdmi-demo) for code that runs a demo over HDMI.
1. Read through the parameters in `console.sv` and tailor any instantiations to your situation.
1. Please create an issue if you run into a problem or have any questions.

### Custom fonts

The default font is the well reputed [Terminus font](https://web.archive.org/web/20080612214835/http://www.is-vn.bg/hamster/jimmy-en.html) in 8x16. You can change the font to one of your liking using [psf2verilog](https://github.com/sameer/psf2verilog) to generate a drop-in replacement for `glyphmap.v`.

### To-do List

* [x] Code point
* [x] Foreground color
* [x] Background color
* [x] Blink
* [ ] Custom font sizes
    * Only fonts with sizes that are multiples of 8 work currently

## Special Thanks

* [Detailed Wikipedia article by Incnis Mrsi](https://en.wikipedia.org/wiki/VGA-compatible_text_mode)
