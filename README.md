# Amp-Space
Scripts, Files, and Resources for Constructing a Large-scale Dataset of Blackbox Effects for Timbre Transfer

## The Amp-Space Project code has been divided into separate repositories to help with distribution:
- [Knoblin](https://github.com/narad/knoblin)

  Knoblin is a (somewhat) user-friendly repackaging of the servo controller aspect of the Amp-Space data collection, used for sampling real devices (guitar pedals, amplifiers).  It has since been updated with a GUI and some improved usability features to help reproduce the configuration used in the Amp-Space paper, across different devices, with different 3D printers, servos, and respective tolerances.
  
- [Tone Render](https://github.com/narad/tone-render)

  Tone Render is a package for generating audio samples from VSTs, performing parameter sweeps in a way analogous to how Knoblin sweeps physical knobs.  Any VST which can be loaded into REAPER should be compatible.  It also includes a set of DI files (both real and synthetic) and scripts to generate scales / note DIs.
  
- Amp-Space Dataset

The Amp-Space Dataset was rebuilt from the ground-up to be more diverse, higher-quality, and user friendly (and to address reviewer concerns) than the originally proposed version.  For distribution, it is currently hosted in separate files, and made available through a HuggingFace Datasets style loader:

https://huggingface.co/datasets/narad/rockingface

Loading the dataset is as easy as:

`from datasets import load_dataset`

`dataset = load_dataset("narad/rockingface")`

It is currently just a test release with a handful of devices, but will be adding more data files once the interface is tested. 


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
