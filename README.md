# Data Science applicata agli Scacchi 

Repository per il progetto di tesi sull'analisi predittiva e feature engineering applicati alle partite di scacchi.

## Come ottenere i dati
Per motivi di spazio, il dataset originale non è caricato su questo repository. Per riprodurre l'analisi:
1. Scarica il file `games.csv` originale da Kaggle (https://www.kaggle.com/datasets/datasnaek/chess)
2. Inserisci il file `games.csv` nella stessa cartella dei notebook su Google Colab.

## Ordine di esecuzione dei Notebook
Per riprodurre l'intero progetto, eseguire i notebook su Google Colab nel seguente ordine:
1. **`01 Pulzia dataset.ipynb`**: Pulizia dati, gestione duplicati, rimozione patte e Analisi Esplorativa (EDA). Salva `train_cleaned.csv` e `test_cleaned.csv`.
2. **`02 Feature_Engineering.ipynb`**: Viene effettuata la feature engeneering, vengono create vari dataset con le colonne aggiunte. Salva i file di addestramento e di test a seconda delle N semimosse analizzate
3. **`03 Baseline.ipynb`**: utilizza i file `train_cleaned_N.csv` e `test_cleaned_N.csv` per definirele prestazioni di riferimento, quindi la baseline dei modelli predittivi che userò dopo, utilizzando tutti i metadati disponibili prima della prima mossa.
