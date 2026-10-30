# Nazra receipt reader models

The text-recognition models Nazra downloads on a phone's first receipt scan. They run on the phone; receipts never
leave it. Nothing else is downloaded from here.

The files are on the [v1 release](https://github.com/alhusamia/nazra-models/releases/tag/v1). The app checks each one
against its SHA-256 before using it:

| File | Size | SHA-256 |
|---|---|---|
| `ch_PP-OCRv5_det_mobile.onnx` (finds the text lines) | 4,819,576 bytes | `4d97c44a20d30a81aad087d6a396b08f786c4635742afc391f6621f5c6ae78ae` |
| `arabic_PP-OCRv5_rec_mobile.onnx` (reads Arabic lines) | 8,023,828 bytes | `c1192e632d0baa9146ae5b756a0e635e3dc63c1733737ebfd1629e87144e9295` |
| `en_PP-OCRv5_rec_mobile.onnx` (reads English lines) | 7,872,351 bytes | `c3461add59bb4323ecba96a492ab75e06dda42467c9e3d0c18db5d1d21924be8` |

## Source and licence

Unchanged copies of the PP-OCRv5 mobile models by [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR), in the ONNX
format published by [RapidOCR](https://github.com/RapidAI/RapidOCR) (release v3.10.0). Both projects are licensed under
the Apache License 2.0; a copy is in [LICENSE](LICENSE). Copyright belongs to the PaddleOCR and RapidOCR authors.
