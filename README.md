# Datatonism

Datatonism is a digital emulation of the Dataton System 3000 – a Swedish electronic music synthesizer. Designed by Björn Sandlund in the 1970s, the system consists of brick-shaped modules that connect to each other sideways like Lego. As final project for the course DT2213 Musical Communication and Music Technology given at KTH Royal Institute of Technology, we have re-created Sandlunds system in a digital context. The name and main patch is dervied from [Automatonism](https://www.automatonism.com/), a modular synth system created for Pure Data.

The system consists of 12 modules – 3 source modules, 5 manipulating modules, and 4 editing modules.

### Requirements / Start-up guide
**Requirements** \
Datatonism is developed on Pure Data. External libraries include `moonlib`.

**Start-up**
- To use Datatonism, you simply download the repository and open the patch called `main.pd`.
- Modules can be found through the MODULES(esc) button or by pressing esc.
- Most modules have 6 inlets and 6 outlets – 2 for the A/B stereo bus and 4 channels. Connections are generally made between the same types, however it is also possible to mix and match.
- The general ordering of inlets/outlets are A, B, ch1, ch2, ch3, ch4.
- **[dac~] is not built in to the mixers and need to be created and connected by yourself.**


### Help-files / [Documentation](https://github.com/kx-shi/Datatonism/wiki)
Help-files for the modules are still a work in process. However, there is [documentation](https://github.com/kx-shi/Datatonism/wiki) covering the inlets/outlets, parameters, and functions of each module, and also a bit about its physical counterpart for the curious.

### Known issues
- Opening module-patches and changing knob parameters can result in the knobs disappearing/become bigger.
- Knobs are not editable in Windows Pd 64-bit version due to constraints from `moonlib`.
- When initially creating modules you might get an error message: "statesave/x-yyy-zzz-ss.txt: can't open / read failed". This is due to the state saving mechanism having to create a file for each new instance of the module and is not a problem.

### Team-members
Dimitrios Aatos Ellinas&emsp;&emsp;&ensp;&nbsp;ellinas@kth.se\
Zezhe Huang&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;zezhe@kth.se\
Kristin Johansson Evegård&emsp;evegard@kth.se\
Carl Leandersson&emsp;&emsp;&emsp;&emsp;&ensp;&ensp;carllea@kth.se\
Martin Linder Nilsson&emsp;&emsp;&emsp;&nbsp;hmni@kth.se\
Karolina Shi&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;karshi@kth.se\
Yan Yu&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;&nbsp;yan8@kth.se
