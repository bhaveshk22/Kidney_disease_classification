
# Kidney-Disease-Classification-MLflow-DVC

## Overview
This project demonstrates the use of transfer learning with the VGG16 model for image classification tasks. The project is structured in a modular fashion, incorporating best practices for machine learning pipelines. We utilize DVC (Data Version Control) to manage our data pipeline and MLflow for tracking experiments and model management.

## Screenshots



![kidneyDisease](https://github.com/user-attachments/assets/d1b41df2-eb0f-4bf0-a09b-3dc2458d8174)


## Features
- **Transfer Learning**: Utilizes the pre-trained VGG16 model.
- **Modular Code Structure**: Organized in a modular fashion for better readability and maintainability.
- **DVC Pipeline**: Manages data and tracks changes effectively.
- **MLflow Integration**: Tracks experiments, logs metrics, and manages model versions.



## Usage
1. **Run App**: Run the app at local host.
    ```sh
    python app.py
    ```

2. **Train Model**: Execute the training script to train the model.
    ```sh
    python main.py
    ```

3. **Data Versioning**: Ensure all data changes are tracked using DVC.
    ```sh
    dvc init
    dvc repro
    dvc dag
    ```


## Project Structure
```plaintext
.
├── data                                            
├── config
│   └── config.yaml                                 
├── research
│   ├── 01_Data_Ingestion.ipynb
│   ├── 02_prepare_base_model.ipynb
│   ├── 03_model_training.ipynb
│   └── 04_model_evaluation_with_mlflow.ipynb
├── src                                             
│   └──cnnClassifier    
│       ├── __init__.py
│       ├── components                                        
│       ├── config
│       ├── constants
│       ├── entity                                      
│       ├── pipeline                                 
│       └── utils                                    
├── dvc.yaml                                        
├── params.yaml
├── app.py
├── main.py
├── requirements.txt                                
├── README.md                                       
└── .gitignore                                      
```

## Workflows
1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline 
8. Update the main.py
9. Update the dvc.yaml
10. app.py

## Lessons Learned
- **Transfer Learning Efficiency**: Using pre-trained models like VGG16 can significantly speed up the training process and improve performance, especially with limited data.
- **Modular Code**: Writing modular code enhances readability, maintainability, and collaboration within a team.
- **Data Management with DVC**: DVC simplifies data versioning and ensures reproducibility in experiments.
- **Experiment Tracking with MLflow**: MLflow provides a powerful framework for tracking experiments, which is crucial for hyperparameter tuning and model selection.

## Contributing
1. Fork the repository.
2. Create a new branch:
    ```sh
    git checkout -b feature/your_feature
    ```
3. Make your changes and commit:
    ```sh
    git commit -m 'Add some feature'
    ```
4. Push to the branch:
    ```sh
    git push origin feature/your_feature
    ```
5. Open a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- [VGG16](https://arxiv.org/abs/1409.1556) for the pre-trained model.
- [DVC](https://dvc.org/) for data version control.
- [MLflow](https://mlflow.org/) for experiment tracking.
- The open-source community for various helpful libraries and tools.

## Authors
[@Bhavesh](https://github.com/bhaveshk22)
