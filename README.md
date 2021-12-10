## MachineTranslation_with_Transformer
- #Data-sets: 5 different data-sets from *Kaggle*.
1. VietNamese to English. The link is [here](https://www.kaggle.com/hungnm/englishvietnamese-translation)
2. English to Vietnamese. The link is [here](https://www.kaggle.com/hungnm/englishvietnamese-translation)
3. English to France. The link is [here](https://www.kaggle.com/digvijayyadav/frenchenglish)
4. France to English
5. English to Italian
- #Frameworks: *Keras*. The pre-train weight is trained on RTX 3060 GPU, hence you need to install CUDA support for tensorflow to load the model. Follow [here]
(https://www.tensorflow.org/install/gpu).
- #Model: Transformer model. This can be based on [keras.io](https://keras.io/examples/nlp/neural_machine_translation_with_transformer/).
- #Evaluation: For Vietnamese to English data-set:
1. Training accuracy: *83.58%*
2. Validation accuracy: *78.60%*
- #Demo and Testing:
The model is deployed using *Flask*, to run and demonstrate the application: 
If you are using anaconda3, do the following:
1. Activate the GPU-environment.
`conda activate [YOUR_GPU_ENVIRONMENT]`
2. Run the `demo.py` file.
`python demo.py`
3. Wait for about 1 minutes for the program to load the model and deploy it on `localhost`.
4. Go to `http://127.0.0.1:5000/` and test the model.
