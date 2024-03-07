# Screen Annotation Dataset

The Screen Annotation dataset consists of pairs of mobile screenshots and their
annotations. The mobile screenshots are directly taken from the publicly
available Rico dataset. The annotations are in text format, and contain
information on the UI elements present on the screen: their type, their
location, the text they contain or a short description. This dataset has been
introduced in the paper
[ScreenAI: A Vision-Language Model for UI and Infographics Understanding](https://arxiv.org/abs/2402.04615)
and can be used to improve the screen understanding capabilities of multimodal
(image+text) models.

## Data split

All the screenshots are split following the splits proposed in
[Screen2Words: Automatic Mobile UI Summarization with Multimodal Learning](https://arxiv.org/abs/2108.03353).

Training, validation and test splits contain 15743 (~70%), 2364 (~10%) and 4310
(~20%) of all screenshots.

## Data format

The data is stored in csv format. Each line contains the following 2 fields:

*   image_id: Screenshot identifier in 
[Rico](http://www.interactionmining.org/rico.html) dataset (should be used to 
get image bytes and other information tied to this screenshot).
*   label: A description of the screenshot that identifies UI elements, their
    type, position, text, and description for images.

The labels were produced using automated techniques, and were verified and
corrected by human raters.

#### Citation

If you use or discuss this dataset in your work, please cite our paper:

```shell
@misc{baechler2024screenai,
      title={ScreenAI: A Vision-Language Model for UI and Infographics Understanding},
      author={Gilles Baechler and Srinivas Sunkara and Maria Wang and Fedir Zubach and Hassan Mansoor and Vincent Etter and Victor Cărbune and Jason Lin and Jindong Chen and Abhanshu Sharma},
      year={2024},
      eprint={2402.04615},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

## License

The dataset is licensed under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

## Contact us

If you have a technical question regarding the dataset or publication, please
create an issue in this repository.