# Llama2-CodeGen
**Fine-Tuning Llama2-7B for Code Generation**

## Overview
Llama2-CodeGen leverages the Llama2-7B model, fine-tuned to generate context-aware Python code from natural language descriptions. This project utilized a custom dataset created by scraping over 25 full-fledged GitHub repositories. The model was initially trained for 100 epochs on a dataset containing 1000 samples, achieving a training accuracy of 89%. With further training and optimization, the model's accuracy was significantly improved.

The project was deployed using Vercel, with a React-based frontend accessible at [projectcodebeing.vercel.app](https://projectcodebeing.vercel.app/).

## Key Features
- **Custom Dataset**: Scraped from over 25 GitHub repositories.
- **Training**: Initial training on 1000 samples for 100 epochs, achieving 89% accuracy.
- **Model Optimization**: Gradual increase in epochs to enhance model performance.
- **Code Formatting**: Integrated black formatting for cleaner output.
- **Deployment**: Hosted on Vercel with a user-friendly React-based frontend.

## Dataset
The dataset used for training is available on Hugging Face:
- [Converted CodeGen Dataset](https://huggingface.co/datasets/Abhiverse01/converted_codegen_dataset.json)

## Training Details
| Parameter             | Value                |
|-----------------------|----------------------|
| Model                 | Llama2-7B            |
| Initial Epochs        | 100                  |
| Initial Training Samples | 1000             |
| Initial Accuracy      | 89%                  |
| Optimizations         | Increased Epochs, Black Formatting |
| Final Deployment      | Vercel               |

## Model Performance
The model showed significant improvements with extended training:
- **Initial Training Accuracy**: 89% after 100 epochs.
- **Enhanced Performance**: With increased epochs, the model's accuracy was greatly improved (assume further specific metrics if needed).

### Training Loss and Accuracy Over Epochs
![Training Curve](path/to/training_curve.png)  
*Figure: Training loss and accuracy curve over multiple epochs.*

## Code Formatting
To ensure the code output is clean and maintainable, black formatting was applied to the generated code. This standardizes the style, making it more readable and consistent.

## Deployment
The project is deployed using Vercel, providing a seamless user experience through a React-based frontend. You can access the live demo here: [ProjectCodeBeing](https://projectcodebeing.vercel.app/).

## How to Use
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/Llama2-CodeGen.git
   ```
2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Model**:
   ```bash
   python generate_code.py --input "Natural language description here"
   ```
4. **Deploy**: Instructions for setting up the Vercel deployment can be found in the `deploy/` directory.

## Future Enhancements
- **Expand Dataset**: Include more diverse repositories to enhance the model's versatility.
- **Fine-Tune for Other Languages**: Adapt the model to support languages other than Python.
- **Interactive Frontend**: Implement an interactive playground on the frontend for live code generation.

## Contributing
Contributions are welcome! Please refer to the `CONTRIBUTING.md` file for guidelines.

## License
This project is licensed under the MIT License - see the `LICENSE` file for details.
