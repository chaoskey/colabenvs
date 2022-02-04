# 已构建环境的分享

https://drive.google.com/drive/folders/1d-CyawFNhJvZeUy0kpHsm4JX44XBtM5q?usp=sharing

务必将这个分享目录`envs`复制到谷歌硬盘的根目录，方便用`./install <环境名>`快速恢复。

在执行后续脚本前，务必先加载谷歌硬盘

```python
# 加载谷歌硬盘
from google.colab import drive
drive.mount('/content/drive')
```

# Gridap环境

```shell
# Gridap初始化安装 或者 已构建环境的恢复
./install Gridap

# 完整的Gridap环境构建【务必在上一步的基础上添加】
./install Gridap add Gridap GridapGmsh GridapODEs ForwardDiff
```

# SciML环境

```shell
# SciML初始化安装 或者 已构建环境的恢复
./install SciML

# 完整的SciML环境构建【务必在上一步的基础上添加】
./install SciML add DifferentialEquations Plots BoundaryValueDiffEq DiffEqBase DiffEqCallbacks DiffEqPhysics OrdinaryDiffEq ParameterizedFunctions RecursiveArrayTools StochasticDiffEq ModelingToolkit SparseArrays SparseDiffTools Sundials SciMLBase Distributions Optim ForwardDiff StaticArrays Latexify NLsolve Unitful SymbolicUtils Symbolics LSODA NeuralPDE DiffEqFlux Flux CUDA DiffEqOperators KernelDensity DiffEqSensitivity Cuba Quadrature CmdStan DiffEqParamEstim AlgebraicMultigrid SparsityDetection BenchmarkTools DiffEqDevTools Catalyst DiffEqUncertainty NLopt DoubleFloats Decimals DecFP Measurements MCMCChains ArbNumerics Turing DynamicHMC TransformVariables DiffEqBayes DiffEqGPU StatsPlots
```

