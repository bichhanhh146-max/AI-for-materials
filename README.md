# Thermal Conductivity Prediction of Thermoelectric Materials

Dự án dự đoán **độ dẫn nhiệt (TC)** của vật liệu nhiệt điện bằng Machine Learning (ML), Multilayer Perceptron (MLP) và Crystal Graph Convolutional Neural Network (CGCNN).

## Dữ liệu

- **20220801_rawdata.csv**: Dữ liệu thô từ StarryData.
- Nguồn dữ liệu: https://github.com/starrydata/starrydata_datasets/blob/master/datasets/20220801.zip
- **data_semiconductor.csv**: Tập dữ liệu tham chiếu trong quá trình xử lý.

## Notebook

- **processing_data.ipynb**
  - Tiền xử lý và làm sạch dữ liệu.

- **collect_CIF_file.ipynb**
  - Thu thập file CIF từ Materials Project thông qua MP API.

- **TC_semiconductor_composition_only.ipynb**
  - Dự đoán TC bằng các mô hình Machine Learning truyền thống.

- **TC_MLP.ipynb**
  - Dự đoán TC bằng mô hình Multilayer Perceptron.

- **TC_CGCNN.ipynb**
  - Dự đoán TC bằng Crystal Graph Convolutional Neural Network.

- Code dự đoán vật liệu mới được tích hợp trong notebook CGCNN.
## Mô hình đã huấn luyện

- ML: **best_model_starry.pkl**
- MLP: *Coming soon*
- CGCNN: **best_cgcnn_tc_temperature_fixed.pt**, **cgcnn_tc_graphs_fixed.pt**
