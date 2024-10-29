# TrafAlert live analysis app

This repo contains the live video analysis app for TrafAlert project,
based on the Savant object detection framework [].

More details to follow.

## How to run

1. Clone the repo
2. Run `git lfs pull` to download the model.
3. Run `docker compose up`.

On first run, it will take a few minutes to build the TensorRT engine for the model,
and to download a sample video from Savant which is run through the pipeline.

The output video is visible live at:

- `http://localhost:8889/stream/source` (WebRTC, open with browser)
- `rtsp://localhost:554/stream/source` (RTSP stream)
