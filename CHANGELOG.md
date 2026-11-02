# FRESCO (TimSlendebroek fork) changelog

This fork is part of the FUSE design stack (see github.com/TimSlendebroek/FUSE_Design.jl). Versions are
`<upstream version at the split>+design.<n>`; they satisfy the same compat bounds as the upstream version and never
clash with upstream release numbers. Releases are git tags `v<version>`.

## 0.7.3+design.1 (2026-11-02, branch `lean-deps`)

Upstream v0.7.3 plus:

- Plots dependency dropped: debug plots use the RecipesBase stubs and only run when Plots is loaded, so FUSE
  workers load FRESCO without Plots.
- Test that FRESCO loads and runs without Plots.
