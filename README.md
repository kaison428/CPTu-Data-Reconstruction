# CPTu-Data-Reconstruction
Data Imputation and denoising using Ensemble Convolutional Autoencoder.

## Introduction

CPTu tests are widely used to determine the properties of soft soils, including clay, fine sand, and silt. The tests measure Cone Tip Resistance (CTR), Sleeve Friction Resistance (SFR), and Pore Water Pressure (PW). However, missing CPTu data is common due to subsurface obstructions. This project proposes an ensemble convolutional autoencoder model using Deep Image Prior (DIP) to impute CPTu data.

## Data Processing

The CPTu data is embedded into a 2D matrix by slicing the 3D spatial data into 2D planes. Missing values are initially imputed with K-Nearest Neighbor (KNN) during data processing. Two input matrices are constructed by filling the missing values with zeros and KNN imputed values.

<p align="center">
  <img src="http://some_place.com/image.png](https://github.com/kaison428/CPTu-Data-Reconstruction/assets/38864087/d79eec73-3067-469a-b0ee-a040c34a847a" />
</p>
 
## Model

The task of data imputation is performed using a convolutional autoencoder. The outputs produced by two different input matrices are linearly combined by an ensemble layer.

## Results

The model was tested and compared to the baseline for all measurement types at a wide range of missing rates. The results demonstrate that the proposed method can achieve better imputation accuracy and robustness compared to the baseline methods.

<p align="center">
  <img src="https://github.com/kaison428/CPTu-Data-Reconstruction/assets/38864087/888a6872-10cb-4c24-844d-61157f58c4fd" />
</p>

## Conclusion

The proposed CPTu data imputation method based on an ensemble convolutional autoencoder can reduce the number of tests required and improve the soil profiling accuracy in case of missing data.

## References

The document includes several references for further reading and understanding.

