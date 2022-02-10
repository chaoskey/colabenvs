# 已构建环境的分享

https://drive.google.com/drive/folders/1d-CyawFNhJvZeUy0kpHsm4JX44XBtM5q?usp=sharing

务必将这个分享目录`envs`复制到谷歌硬盘的根目录，方便用`./install <环境名>`快速恢复。

在执行后续脚本前，务必先加载谷歌硬盘

```python
# 加载谷歌硬盘
from google.colab import drive
drive.mount('/content/drive')

# 获得安装脚本
!cp -p /content/drive/MyDrive/envs/install install
!chmod +x install

# 如果有SciMLGridap环境备份，安装耗时大概2-4分钟
# 如果没有SciMLGridap环境备份，详见 【SciML+Gridap环境】
!./install SciMLGridap
```

# Gridap环境

```shell
# Gridap初始化安装 或者 已构建环境的恢复
# 如果有Gridap环境备份，安装耗时大概 0 分 39 秒
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

# SciML+Gridap环境

```shell
# 如果有SciMLGridap环境备份，安装耗时大概2-4分钟
# 如果没有SciMLGridap环境备份，执行完此步，务必执行下一步
./install SciMLGridap

# 安装耗时大概30-40分钟
# 在SciML基础上安装Gridap
./install SciMLGridap add DifferentialEquations Plots BoundaryValueDiffEq DiffEqBase DiffEqCallbacks DiffEqPhysics OrdinaryDiffEq ParameterizedFunctions RecursiveArrayTools StochasticDiffEq ModelingToolkit SparseArrays SparseDiffTools Sundials SciMLBase Distributions Optim ForwardDiff StaticArrays Latexify NLsolve Unitful SymbolicUtils Symbolics LSODA NeuralPDE DiffEqFlux Flux CUDA DiffEqOperators KernelDensity DiffEqSensitivity Cuba Quadrature CmdStan DiffEqParamEstim AlgebraicMultigrid SparsityDetection BenchmarkTools DiffEqDevTools Catalyst DiffEqUncertainty NLopt DoubleFloats Decimals DecFP Measurements MCMCChains ArbNumerics Turing DynamicHMC TransformVariables DiffEqBayes DiffEqGPU StatsPlots Gridap GridapGmsh GridapODEs
```

# 其它的环境

详见: https://fem-on-colab.github.io/packages.html

我已将其集成为:

```shell

# 1 分 42 秒
./install FEniCS

# 2 分 14 秒
./install FEniCSx  # 默认real模式
./install FEniCSx real
./install FEniCSx complex

# 2 分 48 秒
./install firedrake  # 默认real模式
./install firedrake real
./install firedrake complex

# 0min 38s
./install gmsh

# 2 分 46 秒
./install ngsolve
```

