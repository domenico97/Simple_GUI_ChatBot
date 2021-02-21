# Simple_GUI_ChatBot

# Implementazione di un chatbot tramite l'utilizzo di PyTorch.
Semplice implementazione di un chatbot con PyTorch.

- L'implementazione è piuttosto semplice da seguire e fornire una conoscenza di base dei chatbot.
- L'implementazione utilizza una semplice rete neurale Feed Forward con solo 2 Hidden layer.
- L'esempio è molto personalizzabile. Basta modificare `intents.json` con possibili modelli e risposte e rieseguire l'addestramento (vedi sotto per maggiori informazioni).
- Viene fornita una GUI semplice per l'interazione con il ChatBot. 
    [(ChatBot_GUI_image)](https://github.com/domenico97/Simple_GUI_ChatBot/blob/main/GUI_CharBot_image.png)



Questo approccio è insipirato al seguente articolo: [https://chatbotsmagazine.com/contextual-chat-bots-with-tensorflow-4391749d0077](https://chatbotsmagazine.com/contextual-chat-bots-with-tensorflow-4391749d0077).

## Installazione

### Creare un environment
Qualunque cosa tu preferisca (ad esempio "conda")
Per creare un environment con una specifica versione di Python:
  ```console 
  conda create -n myenv python=3.7 
  ```
  
### Attivare l'environment
 ```console 
 conda activate myenv
   ```

### Installare PyTorch e le dipendenze
Per l'installazione di PyTorch [sito ufficiale] (https://pytorch.org/).
Per installare ntlk: 
```console
pip install nltk
 ```

Se si riscontra un errore durante la prima esecuzione, bisogna anche eseguire l'installazione `nltk.tokenize.punkt`:
Esegui queste istruzioni nel terminale:
 ```console
$ python
>>> import nltk
>>> nltk.download('punkt')
```

## Utilizzo
Run
```console
python train.py
```
Questo porterà alla creazione del file `data.pth`. Dopodiché eseguire questo ulteriore comando:
```console
python chatGUI.py
```

## Note 
Nel caso venga modificato il file `intents.json` sarà necessario rieffettuare il training. Modificando tale file sarà possibile creare un chatbot personalizzato per uno specifico caso d'uso.
