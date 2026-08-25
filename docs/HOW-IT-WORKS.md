# How YouTube Content Works

The visuals on this page are static SVGs, so they render directly on GitHub on phones and desktop browsers. Each one is generated from a model specific to this skill.

## System architecture

![Detailed system map for YouTube Content](../assets/system-map.svg)

### Components

- **1. YouTube URL:** participates in resolve the canonical video and metadata.
- **2. Transcript and timestamps:** participates in fetch or derive timestamped transcript text.
- **3. Claim and topic extractor:** participates in identify sections claims examples and quotes.
- **4. Content transformer:** participates in build a faithful structured summary.
- **5. Source-linked draft:** participates in adapt into thread or blog form.

## Actor and data sequence

![Actor and data sequence for YouTube Content](../assets/operation-sequence.svg)

### 1. Resolve the canonical video and metadata

**Primary surface:** `YouTube URL`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 2. Fetch or derive timestamped transcript text

**Primary surface:** `Transcript and timestamps`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 3. Identify sections claims examples and quotes

**Primary surface:** `Claim and topic extractor`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 4. Build a faithful structured summary

**Primary surface:** `Content transformer`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 5. Adapt into thread or blog form

**Primary surface:** `Source-linked draft`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 6. Retain timestamp links and uncertainty

**Primary surface:** `YouTube URL`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.

## Example output shape

![Illustrative output for YouTube Content](../assets/example-output.svg)

The example is a visual contract: a real run may look different, but it should expose comparable state, provenance, and verification information. It is not presented as evidence of a live external action.

## Decision and stop conditions

![Decision guide for YouTube Content](../assets/decision-guide.svg)

The workflow stops when the target is ambiguous, the relevant surface is unavailable or unauthorized, or the final artifact cannot be checked. A logged-in session or successful tool call is not by itself proof that the requested outcome is complete.

## Verification checklist

- Confirm every component shown in the system map exists in the target environment.
- Trace the actor sequence using actual tool output or artifact state.
- Compare the result with the example-output information contract.
- Re-read or reopen the final artifact instead of trusting an attempt message.
- Report omitted stages, unsupported capabilities, and remaining human decisions.
