# Agent notes

- `origin` is David's fork; `kinesis` is upstream. Most keymap commits come from
  the web keymap editor (keymap-editor[bot]) straight to `origin/V3.0`, so fetch
  and fast-forward before editing locally.
- Firmware is built by GitHub Actions on push to `V3.0` (artifacts
  `firmware-clique` / `firmware-no-clique`). A local `make` build needs Docker
  or Podman running.
- Layer 1 (`gaming`) only overrides the left thumb Space and Esc with plain
  keys, because the hold-tap versions on the base layer misbehave in games. The
  key left of H (`&tog 1` on the base layer, `&trans` on `gaming`) toggles it.
  Layer indices are referenced by number (`&tog 1`, `&lt 3`, `&mo 4`,
  `&tog 5`, `&to 1`), so insert new layers at the end.
