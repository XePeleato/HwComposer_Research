# HiSilicon HwComposer resources

## About

It has been proven that a great number of android HAL modules and kernel drivers from HiSilicon Kirin devices are 'heavily inspired' on Qualcomm's implementations, but the HwComposer module is an exception. The kernel framebuffer driver is somewhat similar to the one present in Qcom kernels, but the userspace module is too different to find a relation between Qcom's userspace driver and our kernel driver.

That's the reason why this repository exists, its goal is to share my IDA database in order to reverse engineer some relevant functions that will empower us to finish the opensource HwComposer module.

## How can I help?

Download the IDA database and decompile whatever you can, or open an issue if you have information that may be relevant, every contribution is appreciated, because this will not just be useful for a single device, but for a handful of custom roms.

## There are like ~1000 functions, are you looking for something concrete?

Yes, every Kirin chipset has its own functions, and right now I am interested in the ones related to Overlay composition (Hi365xOverlay, Hi62XXOverlay...) However note that in your HwComposer library there will be just the functions related to that device, so there will be a folder for each platform.

As a reference, I'll start with the Hi365X HwComposer, so if you're interested to have support on your Hi363X or Hi625X rom just file a new pull request with your HwC library to get it started.

Copybit is also interesting, so relevant information about it is appreciated.
