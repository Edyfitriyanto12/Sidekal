# SIDEKAL : Sistem deteksi kandungan logam & non logam pada proses pengemasan makanan

## Project Description
 Sistem Deteksi Kandungan Logam dan Non-logam (SIDEKAL) dalam proses pengemasan makanan adalah teknologi vital yang digunakan dalam industri makanan untuk memastikan keamanan produk sebelum didistribusikan ke konsumen. SIDEKAL menjadi krusial karena potensi terjadinya kontaminasi logam pada produk makanan selama proses produksi itu sangat besar. SIDEKAL diintegrasikan dengan memanfaatkan Programmable Logic Controller(PLC) dimana sistem dirancang menggunakan konveyor otomatis yang dilengkapi dengan sensor canggih untuk mengidentifikasi keberadaan logam atau non-logam dalam produk makanan pada tahap pengemasan. Hal ini bertujuan untuk memastikan produk yang diproduksi bebas dari kontaminasi sebelum mencapai tangan konsumen.
## Contributor
| Full Name | Affiliation | Email | Role |
| --- | --- | --- | --- | --- |
| Chalda Bhakti Jelika | Ahmad Dahlan University| chalda2115022030@webmail,uad.ac.id | Team Lead |
| Edy Fitriyanto | Ahmad Dahlan University | edy2100022030@webmail.uad.ac.id |Team Member |
| Haris Imam Karim Fathurrahman, S.Pd., M.Sc.| lecturer Ahmad Dahlan University | haris.fathurrahman@te.uad.ac.id |  | lecturer |

## Setup
### Prerequisite Packages (Dependencies)
- pytorch==2.1.0+cu118
- sklearn==1.2.2
- PIL==9.4.0
- matplotlib==3.7.1
- numpy==1.23.5
- streamlit==1.28.2

## Dataset
The Dataset is a manually curated collection of high-quality facial images representing each team member, designed for training and evaluating a face recognition model
- Link: https://drive.google.com/file/d/1F5aAY3sl3X8otpcknJKCEGq-g0SLmZWg/view?usp=sharing

example dataset :

![data ghulam](https://github.com/valentingea/face-recognition-locker-system/assets/117613132/2799604c-a994-41af-ba30-ca2539575979)

## Results
### Model Performance
This section is an overview of the performance of our fine-tuned VGG16 model on a custom dataset. The primary objective was to achieve optimal classification accuracy for images across various classes. The model was trained using different hyperparameter configurations, and we assess its effectiveness through key performance metrics.
Describe all results found in your final project experiments, including hyperparameters tuning and architecture modification performances. Put it into table format. Please show pictures (of model accuracy, loss, etc.) for more clarity.

#### 1. Metrics
The table below summarizes the model's performance across different experiments

| model | epoch | learning_rate | momentum | batch_size | optimizer | train_accuracy | val_accuracy |
| --- | --- | --- | --- | --- | --- | --- | --- |
| vgg16 | 5 | 0.001 | - | 32 | Adam | 97% | 96% | 
| vgg16 | 5 | 0.001 | 0.9 | 43 | SGD | 98% | 97% |
| vgg16 | 5 | 0.01 | 0.9 | 43 | SGD | 97% | 96% |
| vgg16 | 10 | 0.01 | - | 43 | Adagard | 96% | 98% |

#### 2. Ablation Study
Improvements or modifications of our base model vgg16 that we use :
- Freezing Convolutional Layers
- Customized Classifier

#### 3. Training/Validation Curve
Training and validation loss function curve

![loss](https://github.com/valentingea/face-recognition-locker-system/assets/117613132/e9957ea7-6050-45a4-ad8b-ba2b8122ff87)

Training and validation accuracy curve

![akurasi](https://github.com/valentingea/face-recognition-locker-system/assets/117613132/5d5e8b31-f0ba-472d-b4e6-57ad5effc5d9)
 
### Testing
The data we use for testing is data that has been adjusted to the format in deployment. 10 data in testing gave appropriate results.

### Deployment
Our deployment leverages Streamlit, a powerful Python library for creating interactive web applications, to facilitate the seamless and user-friendly selection of lockers based on facial recognition.

![hal 1](https://github.com/valentingea/face-recognition-locker-system/assets/117613132/f002bc0c-94ed-4b0b-bd89-1809ccb37f0a)
![hal 2](https://github.com/valentingea/face-recognition-locker-system/assets/117613132/265cd03d-782d-4f40-ade8-5573cd81b8a7)
![hal 3](https://github.com/valentingea/face-recognition-locker-system/assets/117613132/e012fcd0-8671-4703-8a7e-732dbea0078e)

if you want to try running the program with original data, you can download the model [here](https://drive.google.com/file/d/1sO6vQMFZmZaV3uD47ovzGRN8LuQ55hGf/view?usp=sharing). But, if you want to use your own data, you have to retrain the model with your data.

## Supporting Documents
### Presentation Deck
[Presentation Deck](https://drive.google.com/file/d/1ourl5lYNiHLecRYxaus7g-81wTnnRMXT/view?usp=sharing)

### Business Model Canvas
The business model canvas is a strategic management tool that provides a visual framework for developing, describing, and assessing a business model in a concise one-page format.
![bmc 1](https://github.com/valentingea/face-recognition-locker-system/assets/117613132/ca601234-0514-4e1b-9480-4e294afcca02)
![bmc 2](https://github.com/valentingea/face-recognition-locker-system/assets/117613132/3168af70-21fe-4caa-9822-8c2a638ffbd4)

### Short Video
[Short Video](https://drive.google.com/file/d/11GRKILC0B2dW9ttjJQZ0YE1K5kWBUXeA/view?usp=sharing)

## References
Provide all links that support this final project, i.e., papers, GitHub repositories, websites, etc.
- Link: https://www.kaggle.com/code/nandinibagga/face-recognition-model-opencv-lbph
- Link: https://www.kaggle.com/code/vinayakshanawad/celebrity-face-recognition-vggface-model
- Link: https://...

## How to Cite
If you find this project useful, we'd grateful if you cite this repository:
```
@article{
...
}
```

## License
For academic and non-commercial use only.

## Acknowledgement
This project entitled <b>"YOUR PROJECT TITLE HERE"</b> is supported and funded by Startup Campus Indonesia and Indonesian Ministry of Education and Culture through the "**Kampus Merdeka: Magang dan Studi Independen Bersertifikasi (MSIB)**" program.
