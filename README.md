# AI Refrigerator Inventory System

## Project status

This repository is an early scaffold, not a runnable inventory application. The repository description expresses an intended smart-refrigerator concept, but the currently tracked files do not implement camera-based item recognition, weight-sensor integration, expiry prediction, shopping-list generation, reminders, or ESP32/Raspberry Pi communication.

## Files currently present

| Path | Contents |
|---|---|
| **README.md** | Project status and documentation |
| **requirements.txt** | Flask, OpenCV for Python, NumPy, plus a placeholder comment |

The inspected root tree does not contain Python application modules, a Flask entry point, trained model weights, a dataset, configuration, microcontroller firmware, wiring diagrams, or a bill of materials. There is therefore no application command to run and no hardware build procedure to follow yet.

## Environment setup

The listed Python packages can be installed into an isolated environment, but installing them does not create the missing application.

### Windows PowerShell

    py -m venv .venv
    .\.venv\Scripts\Activate.ps1
    python -m pip install --upgrade pip
    python -m pip install -r requirements.txt

### Linux or macOS

    python3 -m venv .venv
    source .venv/bin/activate
    python -m pip install --upgrade pip
    python -m pip install -r requirements.txt

If PowerShell blocks environment activation, use the platform's standard virtual-environment activation guidance rather than changing machine-wide execution policy just for this project.

The dependency file does not pin versions, so installs may resolve to different package releases over time. Do not interpret a successful package installation as proof that the refrigerator system works.

## Work needed before the concept can be demonstrated

1. Add a real application entry point and define the data model for inventory items.
2. Document the camera and image-processing pipeline, including any model, model license, and dataset requirements.
3. Add the selected weight sensor, ADC/load-cell interface, wiring, calibration procedure, and firmware if hardware is part of the implementation.
4. Specify how expiry dates are supplied or inferred and how uncertain predictions are presented.
5. Document any database, notification service, network protocol, and local configuration required.
6. Add reproducible tests with sample data and clearly separate simulated results from physical hardware results.

Do not connect sensors or buy components based solely on the repository name; the current tree does not specify a verified hardware design.

## Verification status

- The root file list, README, and requirements file were inspected.
- No application code or model was available to run.
- No dependency installation, model inference, camera test, firmware build, or hardware test was performed as part of this documentation update.

## Maintenance & Audit

- **Audit date:** 19 November 2026
- **Documentation status:** README reviewed and audit record added on this date.
- **Scope and evidence:** This is a documentation-level maintenance pass. It does not establish that source code compiles, dependencies are current, security has been tested, or hardware/runtime behavior has been verified.
- **Code and tests:** No new functional code changes or test results are claimed by this README update. Run project-specific build, test, and hardware/runtime checks before relying on the project.
- **Maintenance baseline:** Documentation status recorded through 11 November 2026; revisit setup instructions, dependencies, known limitations, and tests when the project changes.

## Contact

Maintained up to 25 November 2026.

If you encounter any problems, please contact [carmodbhai@gmail.com](mailto:carmodbhai@gmail.com).
