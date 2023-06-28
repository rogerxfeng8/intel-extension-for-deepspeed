# Intel® Extension for DeepSpeed*
Intel® Extension for DeepSpeed* is an extension that brings Intel GPU (XPU) support to DeepSpeed(https://github.com/Microsoft/DeepSpeed). It comes with the following components:
1. DeepSpeed Accelerator Interface implementation
2. DeepSpeed op builder implmentation for XPU
3. DeepSpeed op builder kernel code

DeepSpeed would automatically use Intel® Extension for DeepSpeed* when it is installed as a python package.   After installation, models ported for DeepSpeed Accelerator Interface that run on DeepSpeed could run on Intel GPU device.

## Installation

Optional: need to install [oneAPI Base Toolkit Packages](https://www.intel.com/content/www/us/en/developer/tools/oneapi/base-toolkit-download.html) when using Kernel Injection for inference

`Intel® oneAPI DPC++/C++ Compiler` is required by OP builders to support the JIT build for Kernel Injection.

1. Install Intel® Extension for DeepSpeed*
```python
pip install intel-extension-for-deepspeed
```
 Or, you can build from source:
```python
source ${DPCPPROOT}/env/vars.sh
python setup.py install
```
Generally, DPCPPROOT is /opt/intel/oneapi/compiler/latest for root account, ${HOME}/intel/oneapi/compiler/latest for other accounts.

2. Install DeepSpeed

```python
pip install deepspeed
```
## Get Started
Refer to [examples](https://github.com/intel/intel-extension-for-deepspeed/tree/main/examples#readme)


## Security Policy
Please report security issues or vulnerabilities to the [Intel Security Center].

For more information on how Intel works to resolve security issues, see
[Vulnerability Handling Guidelines].

[Intel Security Center]:https://www.intel.com/security
[Vulnerability Handling Guidelines]:https://www.intel.com/content/www/us/en/security-center/vulnerability-handling-guidelines.html
