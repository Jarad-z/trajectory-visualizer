# ATIF tool-call turn examples

Both files are synthetic ATIF-v1.7 trajectories for the same fictional task.
Upload either JSON file through **Upload OpenHands Trajectory** in the visualizer.

- `atif-same-turn.json`: agent step #2 has three `tool_calls`. The interface shows **Agent turn 1** and **Call 1 of 3**, **Call 2 of 3**, **Call 3 of 3** in one card. Its observation results are deliberately out of order to show that `source_call_id` matches each `tool_call_id`.
- `atif-separate-turns.json`: agent steps #2, #3, and #4 each have one `tool_calls` entry. The interface shows three consecutive cards labeled **Agent turn 1**, **Agent turn 2**, and **Agent turn 3**.

The boundary is the `steps` array, not the time gap between calls. Consecutive calls in one step belong to the same ATIF turn; calls in different steps belong to different ATIF turns.
