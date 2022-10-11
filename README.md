# Genomic Data Processing and Visualization in R (My talk in 2022)
[Link to the slides][gh-pages].

[gh-pages]: https://blog.liang2.tw/2022Talk-genomics-heatmap/
[workflow-status]: https://github.com/ccwang002/2022Talk-genomics-heatmap/actions/workflows/publish.yml


## Abstract
R/Bioconductor provides a powerful ecosystem to conduct genomic analysis in a standardized way.
Together with the strong plotting libraries in R, it's easy to visualize the high dimension of biological data.
Common visualizations include heatmaps and plotting along genomic coordinates.
In this talk, I will cover R's ecosystem for genomics and the related plotting libraries, including packages like GenomicRanges, ensembldb, SummarizedExperiment, and ComplexHeatmap.
We will then go through a series of examples using a brain tumor multi-omics dataset.
First, we will load the dataset and demonstrate how to query the related biological information using these packages.
We will then walk through some interesting biological observations (e.g., X-inactivation and MGMT inactivation) by exploring our data with different visualizations.
Finally, I will share my lessons with R’s overall ecosystem and how it might adapt to the future technologies and new usage.

R/Bioconductor 提供了一個強大並標準的基因數據分析環境。搭配 R 豐富的繪圖套件，很容易能視覺化高維度的生物資訊。常見的視覺化方法包含了 heatmap 和基因體坐標上的作圖。在本次分享中，我將介紹 R 與基因體學相關的資料處理套件和繪圖庫，如 GenomicRanges、ensembldb、SummarizedExperiment 和 ComplexHeatmap 等等。我們將用一個腦癌的資料來示範。首先，我們會用這些套件來輸入 multi-omics 資料並連結相關的資訊和標記。接著，我們會用不同的視覺化方法來探索數據，在其中找尋一些有趣的生物現象（如：X 染色體去活化、MGMT 甲基化）。最後，我將分享我過去幾年使用 R 處理基因資料的經驗，以及它可能如何適用於未來的技術和需求。


## How to build the slides
[![Page build status](https://github.com/ccwang002/2022Talk-genomics-heatmap/actions/workflows/pages/pages-build-deployment/badge.svg)][workflow-status]

First, set up the node.js environment:

    npm install     # Install the dependencies
    npm start       # Start live reloading by browsersync
    npm test        # Run CSS style check using stylelint

To publish the bundled presentation to GitHub Pages, run:

    npm run bundle      # Create standalone bundle
    npm run publish     # Push the bundle to GitHub Pages

This repo also sets up the GitHub workflow that will automatically bundle and publish the presentations on every git push.
The workflow produces a bundled presentation as a compressed file `slides.zip`.

The bundled presentation contains a standalone webpage that can be viewed offline.
Simply open the file `index.html` in a web browser to start the presentation and view the notes.


## License
The theme is shared under [MIT license](LICENSE.md).
It directly modifies the official [Material][Material theme] theme ([the original license][Material license]) and will be in sync with upstream updates.

The theme builds on the following packages and resources:

- Shower's official theme, [Material][Material theme], [MIT License][Material license]
- [Shower]: HTML5 presentation framework by Vadim Makeev *et al.*, MIT license
- [highlight.js]: Code highlighting library by Ivan Sagalaev *et al.*, MIT license
- [KaTeX]: LaTeX math rendering, MIT license
- Fonts:
    - [Source Sans], SIL Open Font License 1.1
    - [Fira Code], SIL Open Font License 1.1

[Material theme]: https://github.com/shower/material
[Material license]: LICENSE.shower_material.md
[shower]: https://github.com/shower/shower
[highlight.js]: http://highlightjs.org/
[KaTeX]: https://github.com/KaTeX/KaTeX
[Source Sans]: https://github.com/adobe-fonts/source-sans
[Fira Code]: https://github.com/tonsky/FiraCode
