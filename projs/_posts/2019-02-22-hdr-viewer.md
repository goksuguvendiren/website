---
layout: project
title: Online HDR Viewer
description: HDR Viewer is here.
class: proj
---

[OpenHDR Viewer](https://viewer.openhdr.org) is the world's first and only online HDR image viewer. We, as a small group in the WMG Visualisation lab
in the University of Warwick, UK, developed the viewer from scratch. The viewer enables changing the exposure of the image,
using different tonemapping techniques, and sharing of the images.

The main idea is that the HDR rendering runs on the client side, and nothing actually gets sent to the server unless the
image is being shared with a third party.

### Implementation Details

The viewer has been built to be run on browsers, and for frontend, we used TypeScript. In the backend, we used C++ for
image reading, *.exr* and *.hdr* image decoding. The C++ code is then compiled into javascript using *Emscripten*.