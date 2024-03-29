# Dataset for the paper "Automatically Prepare Training Data for YOLO Using Robotic In-Hand Observation and Synthesis" 

This repository contains the datasets, models, and test results for the paper "Automatically Prepare Training Data for YOLO Using Robotic In-Hand Observation and Synthesis". We proposed combining robotic in-hand observation and data synthesis to enlarge the limited data set. We first used a robot with a depth sensor to collect images of objects held in the robot's hands and segment the object pictures. Then, we used a copy-paste method to synthesize the segmented objects with rack backgrounds. The collected images and the synthetic ones are combined to train a deep detection neural network. We conducted experiments to compare YOLOv5x detectors trained with images collected using the proposed method and several other methods. The results showed that combined observation and synthetic images led to comparable performance to manual data preparation. They provided a good guide on optimizing data configurations and parameter settings for training detectors. The proposed method required only a single process and was a low-cost way to produce the combined data.

## Changelog
[April 2023] Adding new results for TubeDet

[Oct 2022] Initial release of TubeDet
 
## Setup
Check [YOLOv5](https://github.com/ultralytics/yolov5) repo for details

1. Value the weights by 
```
python .\val.py --weight [weight_option] --img 1376 --data [val_dataset_yaml]
``` 
Change the `[weight_option]` to the path of the weight and change the `[val_dataset_yaml]` to the yaml file of the testing data

2. Value 

## Datasets and Weights

The testing dataset:
| Dataset Names| Dataset links |
| :----: | :----: | 
|Testing Dataset| [Google Drive](https://drive.google.com/file/d/1FVQVKF1bVyt6lNHOO-lNxjRlPzYg6EyE/view?usp=sharing)|
|Testing Dataset (for additional ambient lighting)| [Google Drive](https://drive.google.com/file/d/1bYq46E07PX2YxoxxgJWji24i_g2autWw/view?usp=share_link)|

---

The datasets and weights used in the Table II of the paper.

| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) |[Google Drive](https://drive.google.com/file/d/1Jdg4l6_7SFoGY1qSYZxhF_w7LzRIPYUl/view?usp=sharing) | 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1AG2f6lc4VtoxhoXVwDIqCRV-rSL8N4jA/view?usp=sharing) |
|SR1600| [Google Drive](https://drive.google.com/file/d/1daTh6-bJmTEB591Habbsmqf2PSqsj6AA/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1HHdR2EPa3tlNSJkYzUfaZNNzlgxKqRw5/view?usp=sharing) |
|SB1600|[Google Drive](https://drive.google.com/file/d/1pajWljRSzOhiuK7AvrdopOI2BO10spk7/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1KC80mR-iO4csqmUPfJtQ00MGWK4Jkc9q/view?usp=sharing)|
|RO1600+SR800| [Google Drive](https://drive.google.com/file/d/1WAXnm7OYBK1xFyrRDs8_icCvfAPB7cGQ/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1KmowYCw21mH6TRPa2XQ4xH-_49FAYAmq/view?usp=sharing) |
|RO1600+SB800| [Google Drive](https://drive.google.com/file/d/1o8B8hQQQa5khTG_OIOa2XwTCoRBmp_IU/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1Y9wuuzRPDFNiv4ODmnJa7cKlxFjtpe7W/view?usp=sharing)|
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1VxFnEsCQuVrzLfJOa3vzQNFr2TB87TuD/view?usp=sharing) |
|SR800+SB800| [Google Drive](https://drive.google.com/file/d/1b0EkzFMlH7smpIH_jaBBXfiAuspLCQxB/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1_Tt9h6ojqrt9UtJ4K5IKLTcr4IuJq4DI/view?usp=sharing)| 

---

The datasets and weights used in the Table III of the paper.

| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|RO800+SR200| [Google Drive](https://drive.google.com/file/d/1wjTKqBQW6Qu0KEVwFSHBiGwiAlWSw9fA/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1_41zMDlMU8C7c4XxmkV_SPlb0EnuJlZg/view?usp=sharing)|
|RO800+SR400| [Google Drive](https://drive.google.com/file/d/1s9LjDdTP4ZuoIK2evia3_woCg3JeMsDG/view?usp=sharing)|  [Google Drive](https://drive.google.com/file/d/1Cek4-YR9-3QvfzMKb1INpWeZEFD859pE/view?usp=sharing)|
|RO800+SR800| [Google Drive](https://drive.google.com/file/d/1jjNfqu9m48pkGQTy0s_VAxQzlHKrmNg-/view?usp=sharing)|  [Google Drive](https://drive.google.com/file/d/1Efr4MrvhL_sEMIB6LtlrZwp5bf8kbnOJ/view?usp=share_link)|
|RO800+SR1600| [Google Drive](https://drive.google.com/file/d/1_hTMEwx7mjRFNw1rKI41rE4s4Fv4VHwm/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1cM7bdzI8dElrdC-Ov0Sr8ckeJlBgwwSM/view?usp=sharing)| 
|RO200+SR800| [Google Drive](https://drive.google.com/file/d/107dy_vu5Dbqx76SIBQziP_6Kr7MmOwnn/view?usp=sharing)|  [Google Drive](https://drive.google.com/file/d/1AEStqTVxsyXeYJYHPtyJ_hIJJgzEDoGV/view?usp=sharing)|
|RO400+SR800| [Google Drive](https://drive.google.com/file/d/1sSmkcVVtWgLu3y3haOWOBl4hKpkbMvqD/view?usp=sharing) |  [Google Drive](https://drive.google.com/file/d/1yAZJU1nRK_otMX77qW7zahFAAA6JH9g_/view?usp=sharing)|
|RO800+SR800| [Google Drive](https://drive.google.com/file/d/1jjNfqu9m48pkGQTy0s_VAxQzlHKrmNg-/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1Efr4MrvhL_sEMIB6LtlrZwp5bf8kbnOJ/view?usp=share_link)|
|RO1600+SR800| [Google Drive](https://drive.google.com/file/d/1WAXnm7OYBK1xFyrRDs8_icCvfAPB7cGQ/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1KmowYCw21mH6TRPa2XQ4xH-_49FAYAmq/view?usp=sharing) |

---

The datasets and weights used in the Table IV of the paper.

| Params,(T,t)| Dataset links | Weight links |
| :----: | :----: | :----: |
|(10,.10)| [Google Drive](https://drive.google.com/file/d/11qrU6qkvFCZ4vu9LEy158l1g-GiDZbhA/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1o_Khfpxe0UEO4iSXoypnUImtIg7M5rTl/view?usp=sharing)|
|(20,.10)| [Google Drive](https://drive.google.com/file/d/149lGnaz2ePSJh2kbldaXQMGFyCv_2er0/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1IAp68JWeKUjYOQCTHo348uWO5AlWKxEv/view?usp=sharing)|
|(30,.10)| [Google Drive](https://drive.google.com/file/d/1K2pnUW3obE8VaVGGYukWZmQiQZb-q-Le/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1M7U7ry32nplNEoSmnSevDv_OF_nr_X2k/view?usp=sharing)|
|(40,.10)| [Google Drive](https://drive.google.com/file/d/14lru9jLKaaHkdJquJYvoKmQN-Wn8DzU8/view?usp=sharing)|  [Google Drive](https://drive.google.com/file/d/1j9EUaBhTZMnNUstfiO8JbY1JE4IERLjO/view?usp=sharing)|
|(30,.20)| [Google Drive](https://drive.google.com/file/d/1l-yKUKs1Hwz73W2YAPYex4xD2ttkrghm/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1dLY7pBPKIUBBe4BkkUUHUAGYIXvO22NX/view?usp=sharing)|
|(30,.40)| [Google Drive](https://drive.google.com/file/d/1UWxS2PmXlTKw6KMpxM7in9263M49dGJc/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1x8NJerGezxP__nInmlUjy7HLRT0D-C1M/view?usp=sharing)|
|(30,.60)| [Google Drive](https://drive.google.com/file/d/16-lLsoQaxdndZRKcX4KFo9CFm69OCvQ3/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1aaPNMDYSYnvjsDWC3iB_uLZbZxtNvDdo/view?usp=sharing)|
|(30,.80)| [Google Drive](https://drive.google.com/file/d/106cPWysI56nv_C_3xDABxatPIGjv7AEW/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1y44XvwGUkkSPir61OA8IRbx33hMoIvQE/view?usp=sharing)|

---

The datasets and weights used in the Table V of the paper.

| #Caps| Dataset links | Weight links |
| :----: | :----: | :----: |
|400| [Google Drive](https://drive.google.com/file/d/14qyNUPHDe6f7bT1EX5YOrp-vF4F6gMUr/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/17D99poCkElqfAiOd78Hb1hqtjYh38yIo/view?usp=sharing)|
|800| [Google Drive](https://drive.google.com/file/d/1HxOuIEaejJcEsfHXRZBBzEWlg7NeDQCI/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1GsdH5d00ahdAIt78NJbOJLnbI-DT2B5_/view?usp=sharing)|
|1600| [Google Drive](https://drive.google.com/file/d/15NlkB5oG6gJUU6xSLCvDj5DepJqd_kMj/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/17dHaP3derQzJSi13BGYfdwwfqMQthvmX/view?usp=sharing)|
|3200| [Google Drive](https://drive.google.com/file/d/1b0EkzFMlH7smpIH_jaBBXfiAuspLCQxB/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1_Tt9h6ojqrt9UtJ4K5IKLTcr4IuJq4DI/view?usp=sharing)| 
 
---

The datasets and weights used in the Table VI of the paper.

| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|SB200+SR800| [Google Drive](https://drive.google.com/file/d/1E5BUioUtqmev5qrIPXpp40BgE_lPOlTA/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1og021q1ajWo6cFb4-0VcArNgOmlxaXaV/view?usp=sharing)|
|SB400+SR800| [Google Drive](https://drive.google.com/file/d/13seAmvoGqMM-_KNpYFtNQtbrDctcXeha/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1PwLdCS5Vw0rHBUb9ozFzolyObuh0VDea/view?usp=sharing)|
|SB600+SR800| [Google Drive](https://drive.google.com/file/d/1vg3JWr4QzDVV8waiAllT8-G4prv7tD3L/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1Zh6zCpn9ZZiuOhfZtDnHvp4oVNRVkT0r/view?usp=sharing) |
|SB800+SR800| [Google Drive](https://drive.google.com/file/d/1b0EkzFMlH7smpIH_jaBBXfiAuspLCQxB/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1_Tt9h6ojqrt9UtJ4K5IKLTcr4IuJq4DI/view?usp=sharing)| 
|SB1600+SR800| [Google Drive](https://drive.google.com/file/d/1BeCMifrb4nj5WZO-kF-qFWGK_0dGTUry/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1zhFkIADevgVDdvcVpJ6V_dJPjxUF3Bw-/view?usp=sharing)| 
|SB800+SR200| [Google Drive](https://drive.google.com/file/d/1OQyIEN3ylzVpGz--dFjv725McUl4i9Yt/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/10bHD70o6UPTuFihkYoMOW7EaDbqnlVps/view?usp=sharing)| 
|SB800+SR400| [Google Drive](https://drive.google.com/file/d/11zcDCVs-PgJ5P7fp11u5JdsSblo13R56/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1wQsvuyjEhH6bVr-mu0hRpNAQL6p7-IwC/view?usp=sharing)|
|SB800+SR600|  [Google Drive](https://drive.google.com/file/d/1gktpxa6qpEniMsj8RardqlTBL1bqmucS/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1C1_7Kq2An1MlO20-0HSOYxwdm_ueYaYV/view?usp=sharing)|
|SB800+SR800| [Google Drive](https://drive.google.com/file/d/1b0EkzFMlH7smpIH_jaBBXfiAuspLCQxB/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1_Tt9h6ojqrt9UtJ4K5IKLTcr4IuJq4DI/view?usp=sharing)| 
|SB800+SR1600| [Google Drive](https://drive.google.com/file/d/1FdkHEZSGX9h7dibXWH4iNKudmWphyGaL/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1cv1ZYWzfvknaBIKvxe_N31tMggcQ1LdV/view?usp=sharing)| 

---

The datasets and weights used in the Table VII of the paper
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|_B_| [Google Drive](https://drive.google.com/file/d/1IVfL9btrUVT7l-it_NmLVApe5x9xwBnq/view?usp=share_link) | [Google Drive](https://drive.google.com/file/d/1Qcpq4GK5jwPa38lRYwq2CMx7sOWFO0_o/view?usp=share_link)| 
|_B+_| [Google Drive](https://drive.google.com/file/d/1gzD6utDQMZ9fpn6fEMA6337AxHqMgysa/view?usp=share_link) | [Google Drive](https://drive.google.com/file/d/1VXwuqlruCSmIcaBd6EGeqkWmb8nvuo0U/view?usp=share_link) |
|RO1600 x Cutmix| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/1P3BNeANbitxfxF2K8ytYKtVmaGi69Lue/view?usp=share_link) |
|RO1600 x Mixup| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/1iZ70D2DLbNuliMsm9UrQCpwxbg9_91aO/view?usp=share_link) |

---

The datasets and weights used in the Table IX of the paper

[YOLOv3-SPP](https://github.com/ultralytics/yolov3)
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/1SFim9iLrH0Li7dBvjFLXMVS25OUKaf5n/view?usp=share_link)| 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1x-_7TixIa6AuGx2pCNDTDH8D_521NblG/view?usp=share_link)|
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1VPgfNdDfsI-tXKccKDqTAzWkXLeLxiJ7/view?usp=share_link) |

[YOLOv4](https://github.com/iscyy/yoloair)
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/1i7mjNLh5hNBumiP-Xs_iNV9IYdjZNRrX/view?usp=share_link) | 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1HSTU_SMSbdx6wznTBuMb3czZxaQVS8mH/view?usp=share_link) |
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1hBfaOLa3ZsjiJClwTbM_RoWAIa6Ld3PS/view?usp=share_link)| 

[YOLOv5x](https://github.com/ultralytics/yolov5)
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/1PXOUkEupvSotQdzquLOKMKn2nylKEJmH/view?usp=share_link) | 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1KzM7ynx9hJT01C8bfjxsI1M3pdpFiKQA/view?usp=share_link)|
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1LX-3IPybt-sqnVFVDK2ohO_pqK6pW-GM/view?usp=share_link) |

[YOLOv6-L6](https://github.com/meituan/YOLOv6)
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/12xDS2grmwaeytFwxRV7z7jZjizC67URd/view?usp=share_link) | 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1nhwUFaQ3RdVO_CbTDD6wqfAeGEb9NlYE/view?usp=share_link)|
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1BeqE4IDS2vlwFuA3iiNz4pyYX1-50EpG/view?usp=share_link) |

[YOLOv7-E6E](https://github.com/WongKinYiu/yolov7)
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/1nCFep7nLNxl5r2cA-H3XARO_94EC0E7w/view?usp=share_link) | 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1HiHaqzYZ6pNeX8ARFXLsyxrdjxakpX-t/view?usp=share_link)|
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1lIwKd98aTWIMrebmm4aelCsvtrdQtlHD/view?usp=share_link) |

[YOLOv8x](https://github.com/ultralytics/ultralytics)
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/19kJd9io6PqKSrSiz58HxSgt7iw7Rxub-/view?usp=share_link) | 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1qGi8cJpuVEWfrZVu-AaH5ftwng1A8mdu/view?usp=share_link)|
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1zlh1_mYA_7jqwfI4PMv6usoUcY0QHJlz/view?usp=share_link) |


---

The datasets and weights used in the Table X of the paper

[Faster R-CNN](https://github.com/open-mmlab/mmdetection)
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/1Mr3dqU3KBEcrqoLCWImrlASQ0h4bytLr/view?usp=share_link) | 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1Wh9qu3-rgIxXQM6cpxorrMhX0OfIVbsN/view?usp=share_link)|
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1-tGgYPqDDBh2H70Y3GQACpo7At4Gp1_S/view?usp=share_link) |

[DE:TR](https://github.com/facebookresearch/detr)
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) | [Google Drive](https://drive.google.com/file/d/1dOytl-Uj6kW1J45TflCUUM6Gwdpp1ZV8/view?usp=share_link) | 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1Gpa6JvOJOtAnWJ0HOQy-SCqbI4PIMiUq/view?usp=share_link)|
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1A1VseJU3m08z2HFLzbAfkki_TTOYUaXF/view?usp=share_link) |
