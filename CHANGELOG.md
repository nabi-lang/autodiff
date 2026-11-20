# Changelog

All notable changes to this package. Versions follow semver, independent of the Nabi toolchain.

## 0.1.0 (unreleased)

First release.

- Forward mode: `Dual` (one direction) and `Duals<N>` (`N` directions per
  evaluation).
- `HyperDual` for exact Hessians, `Jet` for derivatives of any order.
- Reverse mode: `Var` on a `Tape`, gradients of many inputs in one backward
  sweep.
- `Smooth`: write a function once and run it in every mode.
- `grad`, `value_grad`, `jacobian`, `value_jacobian`, `hessian`, `jvp`, `vjp`
  and `derivative` / `derivatives`, on any `linalg::AsVector` point.
- The `ops` feature (default): the `ε` suffix and the `∂` / `∇` operators,
  extensible through the `Derive` and `Gradient` traits.
- f64, pure Nabi, every target including wasm. Needs Nabi 0.1 or later;
  depends on `linalg`.
