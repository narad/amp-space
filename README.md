# Amp-Space
Scripts, Files, and Resources for Constructing a Large-scale Dataset of Blackbox Effects for Timbre Transfer

## The Amp-Space Project code has been divided into separate repositories to help with distribution:
- [Knoblin](https://github.com/narad/knoblin)

  Knoblin is a (somewhat) user-friendly repackaging of the servo controller aspect of the Amp-Space data collection, used for sampling real devices (guitar pedals, amplifiers).  It has since been updated with a GUI and some improved usability features to help reproduce the configuration used in the Amp-Space paper, across different devices, with different 3D printers, servos, and respective tolerances.
  
- ReaScripts (Coming soon!)
- Device Sampler (Coming soon!)
- Amp-Space Dataset
  - Synthetic Data
  - Real Data
- Models & Benchmarks


### Reference

The code and data in this repository was originally developed for and described in [Amp-Space](https://www.dafx.de/paper-archive/details.php?id=G8gchE7K8Itm8VPTGRtYyA), an on-going project in machine learning and interface design for music, focused primarily on timbre-changing effects for guitar:

```
@article{narad2021ampspace,
  title = {Amp-Space: A Large-scale Dataset for Fine-grained Timbre Transformation},
  author = {Naradowsky, Jason},
  journal = {Proceedings of the 24th International Conference on Digital Audio Effects (DAFx-21), Vienna, Austria},
  year = {2021}
}
```
