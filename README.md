# WGS Nomenclature Playground

> ⚠️ **Draft proposal — not an official standard.** This is an interactive demo to discuss an
> invariant, decentralised, LINcode-style WGS naming scheme for viral pathogens (illustrated on BTV and WNV).

An interactive, single-file web playground that demonstrates how a **pathogen-agnostic, hierarchical,
threshold-based** nomenclature would work — the same family as LIN / LINcodes, SnapperDB SNP-addresses and HierCC.

**▶ Live playground:** https://genpat-it.github.io/wgs-nomenclature-proposal/

## What it shows

1. **Tree → Code** — from a distance matrix to a hierarchical path-code (`A.B.C`); editable spreadsheet
   matrix, distance histogram, choice of linkage (single / average / complete) and number of levels;
   three views: LIN tree, dendrogram, MST.
2. **Split vs Medoid** — above the threshold → split; below → pick the medoid (the deterministic reference).
3. **Invariance** — frozen backbone vs recompute: why names stay stable, and the blind spots
   (within-threshold novelty, resolution cap), with the distance matrix that explains each case.
4. **Constellation / Reassortment** — segmented genomes (BTV): one code per segment; a reassorted
   segment shows up as an outlier digit.
5. **Central registry vs Invariant** — side-by-side: a central-registry/serial model reshuffles as data
   arrive, the invariant model does not.

## Key idea

The name is a **path down a tree**: shared prefix = shared ancestry. New data only **append** digits;
old names never change (invariance). Everyone recomputes the same code from a **public, versioned backbone
+ thresholds** (decentralised). Distances are an **input** — this tool is only the naming layer.

## Run locally

It is a single static file — just open `index.html` in a browser (Chrome / Firefox). No server, no build.
