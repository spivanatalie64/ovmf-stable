# ovmf-stable

AcreetionOS mirror of the **latest EDK II long-term stable release branch**
(OVMF firmware source), synced into `main`.

- **Upstream:** [tianocore/edk2](https://github.com/tianocore/edk2)
- **Branch synced:** `stable/202508` → `main` (tip matches `edk2-stable202508.01`)
- **Content:** identical to upstream — full commit history of the LTS branch, no other branches or tags

## Re-sync

```sh
git fetch upstream
git merge --ff-only upstream/stable/202508
git push origin main
```

Upstream remote is already configured as `upstream` (tianocore/edk2, tracking
`stable/202508` only). This mirror is read-only by policy — all AcreetionOS
patches land behind us, or upstream first.

## Building OVMF

See upstream `ReadMe.md` or `Build` instructions under `OvmfPkg/`.
