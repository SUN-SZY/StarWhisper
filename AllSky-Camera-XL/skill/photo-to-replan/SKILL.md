---
name: photo-to-replan
description: Use this skill when the user wants to run the end-to-end all-sky photo pipeline from a raw all-sky image to a replanned observing sequence, using the packaged run_pipeline.py entrypoint in this shared directory.
---

# Photo To Replan

Use this skill when the task is to go from a raw all-sky image to replanned observing outputs.

## Workflow

1. Locate the shared `photo_to_replan_pipeline` directory.

2. Run the single-entry pipeline script from that directory:

```bash
python run_pipeline.py --image /abs/path/to/image.jpg
```

Optional:

- Override parameter group with `--position-name position_X`
- Save segmentation overlay with `--save-overlay`

3. Read the generated report:

- `output/<image_stem>/pipeline_report.json`

4. From the report, inspect these outputs when needed:

- `scenario.json`
- `replanned_schedule.json`
- `deferred_targets.json`
- `replanned_sequence.ninaTargetSet`
- `sky_replan_plot.png`

## Input Requirements

- The input must be a raw all-sky camera photo.
- The filename should contain Beijing time, preferably in `YYYY_MM_DD_HH_MM_SS.jpg` form.

## Notes

- The mask stage uses the packaged `Pic2mask/full_image_infer/infer_full_image.py`.
- The replan stage uses the packaged `sequence_adjust_tool/scheme_horizon_to_image/replan.py`.
- The pipeline configuration is stored in `configs/default.json`.
- The packaged configuration uses a single conda environment for the whole pipeline.

## Validation

A run counts as pipeline-successful if these files exist and are readable:

- `pipeline_report.json`
- `scenario.json`
- `replanned_schedule.json`
- `replanned_sequence.ninaTargetSet`

Business success is separate. Check `deferred_targets.json` and `replanned_schedule.json` to see whether future slots were actually filled.
