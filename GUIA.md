# **Melhor Guia de RVC confiado por 100% dos leitores**

### **Links:**

##### **RVC: Treino e clonagem de voz**
- [**Colab do Applio UI**](https://colab.research.google.com/github/iahispano/applio/blob/master/assets/Applio.ipynb) para treinar modelos e fazer inferencias usando interface gráfica.
- [**Colab do Applio No UI**](https://colab.research.google.com/github/iahispano/applio/blob/master/assets/Applio_NoUI.ipynb) para treinar modelos e fazer inferencias usando unicamente interface do Colab.

##### **Separação de vocais e limpeza de áudio**

- [**MVSEP**](https://mvsep.com/pt/home) contém os melhores modelos de separação de vocais e limpeza de áudio. **Se registre para baixar os arquivos em FLAC e ter filas de espera menores**
- [**Colab de modelos de separação**]() contém quase todos os modelos de separação de vocais e limpeza de áudio do MVSEP, pórem, sem filas.

### **1. Separação de vocais (Passo a passo):**
**Importante: Sempre exporte os arquivos de áudio em FLAC!**
##### **1. Remover os instrumentais**

**MVSEP:** Selecione o modelo **"MelBand Roformer"** no primeiro menu, no segundo deixe **"ver 2024.10"**

**Colab:** Selecione o modelo **"VOCALS-MelBand-Roformer Kim FT (by Unwa)"**

##### **2. Remover Backing Vocals:**

**MVSEP:** Selecione o modelo **"MelBand Karaoke"**

**Colab:** Selecione o modelo **"KARAOKE-MelBand-Roformer (by aufr33 & viperx)"**

##### **3. Remover Reverb:**

**MVSEP:** Aqui depende o modelo, se o reverb do áudio for mono, selecione **"Ultimate Vocal Remover HQ"** e **"UVR-DeEcho-DeReverb"**. Se o Reverb for stereo, selecione **"Reverb Removal"** e **"Reverb removal by anvuew v2 (MelRoformer)"**

**Colab:** No colab só tem o modelo para remover reverb stereo, que é o **"DE-REVERB-MelBand-Roformer v2 (by anvuew)"**

##### **4. Remover Eco (Se necessário):**

**MVSEP:** Selecione o modelo **"Ultimate Vocal Remover HQ"** e **"UVR-De-Echo-Normal"**

**Colab:** Nesse colab não tem um modelo específico para remover eco

### **2. Limpeza de áudio (Passo a passo):**

**Em construção!**

### **3. Treino de modelo no Applio UI (Passo a passo):**

Na primeira parte, coloque o **nome do modelo** e coloque o **"Sampling Rate"** em **"32000"**

Na parte de **"extrair"** deixe tudo do jeito que está

Na parte de **"Training"** coloque **"Tamanho do Lote"** em **8** e **"Total de Epochs"** em **300** e inicie o treino. O progresso dos Epochs vai aparecer na página do Colab.
