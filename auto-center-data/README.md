## Introduction

Welcome to the first in a series of After Effects projects and scripts designed to showcase powerful techniques that can expand and customize your experience with Templater. This project demonstrates how our custom plugin can be extended through creative scripting to unlock dynamic, data-driven workflows inside After Effects.

>![Preview of the Auto Center Data Autograf](preview-auto-center-data.png)

## What it Does

This project was developed in response to a specific customer request. For the project in question, the customer had five inputs of names and titles. The names would have titles placed below each layer in a smaller font, and the entire stack would be vertically centered in the project. The main change the customer wanted was for the project to re-adjust the vertical centering if one of the fields was blank. So, if layers 2 and 4 had no data, layers 1, 3, and 5 should adjust to be evenly spaced and vertically centered.

## How it Works

There are two comps in this project file, "names-only" and "names-and-titles". Names-only has five names vertically tiled with a consistent padding between each text layer. Names-and-titles is similar, but each name also has a title layer below it that should line up with the bottom of the preceding layer. 

The main thing that this project does differently is that it incorporates a series of After Effects Expressions on the layers with Alignment Properties, which checks the layer above to see if it's blank and then subtracts the Templater "padding" value from the Position value in the Transform Properties. This causes a blank layer to essentially be "zeroed" out when Templater performs its alignment calculations, which means that blank layers will no longer cause alignment issues.

## Potential Alterations

One of the main challenges to getting this project to work correctly was understanding how to utilize Templater Effects values in conjunction with Expression calculations to make last-minute adjustments to the layout of the project. Once this concept is understood, there's a lot of potential to create more intricate Expressions that make adjustments to Position, Scale, etc. based on what values are present in both the layer data and the Templater Settings Effect.

## Support

Thank you for testing out these Autografs with Templater! If you find they do not work for you, and if the additional learning resources do not help fix the issues you encounter with these Autografs, please feel free to [contact us via Dataclay's support](https://dataclay.com/contact-us/), or simply add an entry to this repository's issues tab.

Happy Rendering!!!