
Welcome!!

## Potential Risks of AI Writing Style Imitation Based on Personal Chat Data/<br/>Potenzielle Risiken der Schreibstil-Imitation durch KI-Modelle anhand persönlicher Messenger-Daten
 
# **Project description** (Eng)

This project represents an attempt to fine-tune an AI model using personal WhatsApp chat data to approximate
a person's specific writing style.

As part of the project, a fine-tuning experiment is conducted using a LoRA configuration.  

For the **training pipeline**, the LLaMA 3.2 3B Base and Instruct models were compared, with the Base model being
primarily used.  
For the **evaluation pipeline**, six different evaluation metrics and a significance test were implemented and used for the evaluation.
- BERTScore
- BLEU
- ROUGE-L
- Answer length
- Emoji count
- Number of non-empty lines
- Wilcoxon signed-rank test

## Technologies
Python · PyTorch · Hugging Face Transformers · PEFT/LoRA · TRL · LLaMA 3.2 3B · CUDA · Jupyter · BLEU · ROUGE-L · BERTScore · scikit-learn

## Structure


llm-personal-sytle-tuning/  
│  
├── notebooks/  
│   ├── A01Data_preparation_and_training.ipynb  
│   ├── A02Training_result_check.ipynb  
│   └── ...  
│  
├── results/  
│   ├── graphs/  
│   ├── tables/  
│   └── ...  
│  
├── data/  
│   
│  
├── models/  
│   
│  
├── README.md  
├── requirements.txt  
└── .gitignore  

**Notebooks:**  
  The six notebooks represent the implementation of the experiment and the evaluation.  

- A) is divided into three parts: The first is data preparation, the second is training, and the third is 
testing the model and the dataset through inference and word clouds.

- B) The other three notebooks make up the evaluation pipeline. "Generate_Answers" generates the candidate texts for 
comparison, "Metrics" calculates the comparison between the models, and "analysis" analyzes and evaluates the results.


**Results:**  
The project results are organized into graphical and tabular outputs.  

## Training Progress
<img width="1190" height="690" alt="Mean_Token_Accuracy1_6" src="https://github.com/user-attachments/assets/fb39fa1a-cae7-4ac8-aca0-fdaf9007e5e9" />
Evaluation of the Mean Token Accuracy over the training attempts



### Evaluation Comparison Base Model vs. Fine-Tuned Adapter  
 
<img width="790" height="490" alt="ComparisonEvaluation" src="https://github.com/user-attachments/assets/52b366cf-5aa6-47f6-83cf-e8ed4a1e943c" /><br> 
Comparison of the Automatic Evaluation Metrics

<img width="690" height="390" alt="AntwortlängeComparisonEvaluation" src="https://github.com/user-attachments/assets/ce0e7e7a-373e-410e-9a57-59997ccfed52" /><br>
Comparison of the length of the answers  

<img width="689" height="390" alt="Herunterladen (1)" src="https://github.com/user-attachments/assets/05c3e09e-6417-4adf-9b5f-83de906cfda3" /><br>
Comparison of the amount of not empty lines


    
# **Projektbeschreibung** (Ger)

Das Projekt stellt den Versuch dar ein Ki-Modell mit persönlichen WhatsApp-Chatdaten zu feinjustieren, 
um eine Annäherung des Schreibstils an die Person zu erwirken.

Im Rahmen des Projekts erfolgt ein Experiment mit Fine-Tunings, das im Rahmen einer LoRA Konfiguration
abläuft.

Für das Trainingspipeline wurden im Experiment die LLaMA 3.2 3b base und instruct Modelle verglichen und das 
base Modell hauptsächlich verwendet.  
Für die Evaluationspipeline wurden sechs verschiedene Evaluationsmetriken und ein Signifikanztest implementiert und verwendet.
- BERTScore
- Bleu
- Rouge-L
- Antwortlänge
- Emoji-Anzahl
- Nicht-leere Zeilenanzahl
- Wilcoxon-Vorzeichen-Signifikanztest

## Technologien
Python · PyTorch · Hugging Face Transformers · PEFT/LoRA · TRL · LLaMA 3.2 3B · CUDA · Jupyter · BLEU · ROUGE-L · BERTScore · scikit-learn

## Struktur

llm-personal-sytle-tuning/  
│  
├── notebooks/  
│   ├── A01Data_preparation_and_training.ipynb  
│   ├── A02Training_result_check.ipynb  
│   └── ...  
│  
├── results/  
│   ├── graphs/  
│   ├── tables/  
│   └── ...  
│  
├── data/  
│   
│  
├── models/  
│   
│  
├── README.md  
├── requirements.txt  
└── .gitignore  

	
**Notebooks:**  
  Die sechs Notebooks stellen die Implementierung des Experiments und der Evaluation dar.
	
- A) ist in drei Teile gegliedert. Der erste ist die
	 Datenaufbereitung. Der zweite ist das Training. Der dritte ist die Testung des Modells
	 und des Datensatzes durch Inferenzen und Wordclouds.

- B) Die weiteren drei Notebooks sind die Evaluationspipeline. "Generate_Answers" generiert 
	 die Kandidatentexte zum Vergleich, "Metrics" berechnet den Vergleich der Modelle und 
	 "analysis" analysiert die Ergebnisse und wertet sie aus.
	

**Results:**  
    Die Ergebnisse des Projekts sind in grafische und tabellarischen Ausgaben gegliedert.
