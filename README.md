![Photo Ink demonstration: a walking person redrawn as an ink-and-wash illustration](examples/ink-person-walking.png)

# Photo Ink

> Transform one authorized photo into one coherent ink-and-wash illustration while retaining its composition, recognisable subjects, and source-derived colour relationships.

[GitHub Repository](https://github.com/Lone3m-tech/smkt-photo-ink) · [简体中文](README.zh-CN.md)

## Current status

This is a public source Skill released under the MIT License. The four source/output pairs in `examples/` are owner-approved, AI-generated demonstrations of the fixed treatment.

No GitHub Release tag or ZIP installer has been created. This repository does not claim universal host compatibility.

## Install

In a host that supports installing Agent Skills from GitHub, ask:

> Please install this Skill: https://github.com/Lone3m-tech/smkt-photo-ink

The host must be able to read the Skill, accept an uploaded image, and perform reference-image editing. Availability depends on that host.

## Get started

Upload a photo you are authorized to transform, then ask:

> Turn this photo into an ink-and-wash illustration.

The Skill returns one complete scene redraw. If no usable photo is provided, it asks for one instead of inventing a source scene.

## How it works

Photo Ink is a fixed treatment, not a multi-style tool. It redraws people, animals, objects, and backgrounds in one visual language while preserving aspect ratio, composition, subject count, poses, major spatial relationships, and source-derived colour families.

The treatment uses warm off-white paper, restrained near-black ink contours, translucent source-colour washes, and open breathing room. It has no style, palette, detail, or subject-lock controls.

## What it does

- Input: one photo you are authorized to transform.
- Output: one complete ink-and-wash illustration, not a partial filter or collage.
- Preserves: recognisable subject features, clothing or animal markings, scene anchors, composition, and major colour relationships.
- Excludes: photographic cutouts, text, labels, logos, watermarks, borders, extra subjects, and distorted anatomy.

## Use cases

- Hand-drawn portrait reinterpretations.
- Full-scene pet-photo redraws.
- Illustration treatments for an object or everyday scene.
- Unified rendering of travel, landscape, city, or interior photographs.

## Who it is for

Creators, content teams, and brand teams that need a consistent hand-drawn interpretation of an existing portrait, pet, object, or scene photo.

## Not for

- Article visual packages, diagrams, text posters, or generating a new scene without a photo.
- Multiple style, palette, detail, or subject-lock options.
- Pixel-identical photo preservation, identity verification, automated visual QA, retries, or variant selection.
- Background swaps or requests that keep a photorealistic subject untouched.

## Core capabilities

- Full-scene consistency: people, animals, objects, and backgrounds are redrawn in one ink-and-wash language.
- Source relationships first: the treatment preserves aspect ratio, composition, subject count, poses, major spatial relationships, and source-derived colours.
- Recognisable interpretation: silhouettes, clothing, markings, and scene anchors support recognition without pixel-level copying.

## Complete demo

The included pairs are owner-approved examples. The source photos were authorized for this demonstration; the Ink results are AI-generated examples. They show the intended fixed treatment, not a guarantee for every image, model, or host.

| Source | Ink result |
| --- | --- |
| ![Walking person source](examples/source-person-walking.png) | ![Walking person Ink result](examples/ink-person-walking.png) |
| ![Cat in fox hood source](examples/source-cat-fox-hood.png) | ![Cat in fox hood Ink result](examples/ink-cat-fox-hood.png) |
| ![Alpine valley source](examples/source-alpine-valley.png) | ![Alpine valley Ink result](examples/ink-alpine-valley.png) |
| ![Three friends source](examples/source-three-friends-low-angle.png) | ![Three friends Ink result](examples/ink-three-friends-low-angle.png) |

## Dependencies and limitations

- Requires image input, Skill instruction reading, and reference-image editing in the host; it does not guarantee support for every host or image model.
- If image editing is unavailable, the Skill reports the blocker instead of inventing an output.
- You are responsible for source-image copyright, portrait, and privacy permissions, and for complying with the terms of the image service you use.
- This is not photo restoration, identity verification, or a guarantee of copyright, privacy, or output-use rights.

## License

[MIT](LICENSE). Contributions and issue reports are welcome through GitHub.
