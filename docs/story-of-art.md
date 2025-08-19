 **bengala inteligente / análise de marcha em AVC**:

---

### 🔹 **1. Gait in Aging and Disease Dataset (PhysioNet)**

* **O que tem:** Dados de marcha coletados em idosos e pacientes com doenças neurológicas. Inclui parâmetros de marcha como comprimento do passo, cadência, variabilidade, etc.
* **Formato:** Arquivos `.txt` com séries temporais.
* **Link:** [PhysioNet - Gait in Aging and Disease](https://physionet.org/content/gaitdb/1.0.0/)

Esse é o mais próximo do seu objetivo (monitorar marcha em populações clínicas).

---

### 🔹 **2. Daphnet Freezing of Gait Dataset**

* **O que tem:** Dados de sensores vestíveis (acelerômetros) em pacientes com **distúrbios de marcha**, principalmente Parkinson.
* Pode servir como **analogia** para AVC, já que captura padrões anômalos de movimento.
* **Formato:** Séries temporais de acelerômetro.
* **Link:** [PhysioNet - Daphnet Freezing of Gait](https://physionet.org/content/daphnet-freezing-gait/1.0.0/)

---

### 🔹 **3. UCI Machine Learning Repository – Gait Recognition Dataset**

* **O que tem:** Medições de marcha de indivíduos saudáveis em diferentes condições.
* Não é clínico (sem AVC), mas ótimo para treinar modelos iniciais.
* **Link:** [UCI Gait Dataset](https://archive.ics.uci.edu/ml/datasets/a+gait+database+for+evaluation+of+anthropometric+and+gait+feature+recognition+algorithms)

---

### 🔹 **4. Kaggle – Gait Recognition Datasets**

No Kaggle existem vários datasets de marcha baseados em visão computacional e sensores. Exemplos:

* [Gait Recognition Dataset](https://www.kaggle.com/cvdf/gait-recognition-dataset)
* [MotionSense Dataset](https://www.kaggle.com/datasets/malekzadeh/motionsense-dataset) (dados de sensores IMU, ótimo para simular a bengala com acelerômetro).

---

⚡ **Sugestão para o notebook inicial**:

* Baixar um desses datasets (ex.: MotionSense ou PhysioNet Gait)
* Carregar no Pandas/Numpy
* Extrair features simples: cadência, variância do tempo entre passos, média da amplitude
* Plotar gráficos comparando “healthy gait” vs “impaired gait”
* Rodar um **classificador simples (RandomForest ou SVM)** para testar se já dá para separar os dois grupos.

---

👉 Quer que eu já monte para você um **notebook inicial (`notebooks/01_data_exploration.ipynb`)** que carrega um desses datasets públicos e faz análise exploratória + modelo básico?
