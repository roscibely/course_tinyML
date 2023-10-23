# Curso de aprendizado de máquina em sistemas embarcados 
_Tiny Machine Learning - TinyML_
###### Professora: [Rosana Rego](https://github.com/roscibely)
--- 

Este repositório abriga uma coleção de slides, material de leitura, solicitações de projetos e exemplos para você começar a criar seu próprio projeto de aprendizado de máquina em sistema embarcado.

### Pré requisitos 

Os alunos devem estar familiarizados com os seguintes tópicos para completar os exemplos de perguntas e tarefas práticas:

* Álgebra
    - Resolvendo equações lineares
* Probabilidade e Estatística
    - Expressando probabilidades de eventos independentes
     - Distribuições normais
     - Média e mediana
* Programação
    - Programação Arduino/C++ (condicionais, loops, arrays/buffers, ponteiros, funções)
    - Programação Python (condicionais, loops, arrays, funções, NumPy)

### Hardware e Software Necessários

Os alunos precisarão de um computador e acesso à Internet para realizar treinamento em modelo de aprendizado de máquina e exercícios práticos com o Edge Impulse Studio e o Google Colab.

* É necessária uma conta do Google para o [Google Colab](https://colab.research.google.com/).

* Um Edge Impulse é necessário para o [Edge Impulse Studio](https://edgeimpulse.com/).

* Os alunos precisarão instalar o [Arduino IDE](https://www.arduino.cc/en/software) mais recente.

## Cronograma de Estudos 

* [Módulo 1: Machine Learning embarcado](#módulo-1-machine-learning-embarcado)
* [Módulo 2: Iniciando com Deep Learning](#módulo-2-iniciando-com-deep-learning)
* [Módulo 3: Fluxo de trabalho com Machine Learning](#módulo-3-fluxo-de-trabalho-com-machine-learning)
* [Módulo 4: Implantação de modelos](#módulo-4-implantação-de-modelos)
* [Módulo 5: Classificação de imagens com aprendizado profundo](#módulo-5-classificação-de-imagens-com-aprendizado-profundo)


### Material de apoio

* [Curso TinyML](https://www.coursera.org/learn/introduction-to-embedded-machine-learning?action=enroll)
* [Arduino Nano 33 BLE Sense](https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense#connecting-an-off-the-shelf-ov7675-camera-module)

--- 


### Módulo 1: Machine Learning Embarcado

Este módulo fornece uma visão geral do aprendizado de máquina e como ele pode ser usado para resolver problemas. Ele também introduz a ideia de executar algoritmos de aprendizado de máquina em dispositivos com recursos limitados, como microcontroladores. 

##### Material


| ID | Descrição | Links | Fonte |
|----|-------------|:-----:|:-----------:|
| 1.1.1 | O que é machine learning | [video](https://www.youtube.com/watch?v=RDGCGho5oaQ&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=3) [slides](Module%201%20-%20Introduction%20to%20Machine%20Learning/1.1.1.what-is-machine-learning.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 1.1.2 | Machine learning em sistemas embarcados | [video](https://www.youtube.com/watch?v=Thg_EK9xxVk&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=6) [slides](Module%201%20-%20Introduction%20to%20Machine%20Learning/1.1.2.machine-learning-on-embedded-devices.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 1.1.3 | O que é tiny machine learning | [slides](Module%201%20-%20Introduction%20to%20Machine%20Learning/1.1.3.what-is-tiny-machine-learning.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |


### Módulo 2: Iniciando com Deep Learning

Este módulo fornece uma visão geral das redes neurais e como elas podem ser usadas para fazer previsões. 

| ID | Description | Links | Attribution |
|----|-------------|:-----:|:-----------:|
| 2.1.1 | O paradigma do aprendizado de máquina | [slides](Module%202%20-%20Getting%20Started%20with%20Deep%20Learning/2.1.1.the-machine-learning-paradigm.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 2.1.2 | Pensando na perda | [slides](Module%202%20-%20Getting%20Started%20with%20Deep%20Learning/2.1.3.thinking-about-loss.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 2.1.3 | Minimizando perdas | [slides](Module%202%20-%20Getting%20Started%20with%20Deep%20Learning/2.1.4.minimizing-loss.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 2.1.5 | Primeira rede neural | [slides](Module%202%20-%20Getting%20Started%20with%20Deep%20Learning/2.1.5.first-neural-network.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |


### Módulo 3: Fluxo de trabalho com Machine Learning

Neste módulo, os alunos compreenderão como os dados são coletados e usados para treinar um modelo de aprendizado de máquina. Eles terão a oportunidade de coletar seu próprio conjunto de dados, carregá-lo no Edge Impulse e treinar um modelo usando a interface gráfica. A partir daí, eles aprenderão como avaliar um modelo usando uma matriz de confusão para calcular precisão, recall, exatidão e pontuações F1.

#### Material


| ID | Descrição | Links | Fonte |
|----|-------------|:-----:|:-----------:|
| 3.1.1 | Aplicações TinyML | [slides](Module%203%20-%20Machine%20Learning%20Workflow/3.1.1.tinyml-applications.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 3.1.3 | Ciclo de vida do Machine learning  | [slides](Module%203%20-%20Machine%20Learning%20Workflow/3.1.3.machine-learning-lifecycle.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 3.1.3 | Coletando dados com Edge Impulse | [video](https://www.youtube.com/watch?v=IiJKqHRRuD4&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=9) [slides](Module%203%20-%20Machine%20Learning%20Workflow/3.2.6.data-collection-with-edge-impulse.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |

#### Treinando e validando o modelo de ML 


| ID | Descrição | Links | Fonte |
|----|-------------|:-----:|:-----------:|
| 3.2.1 | Extração de recursos (_features_) | [video](https://www.youtube.com/watch?v=oDFxBjcvrQU&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=10) [slides](Module%203%20-%20Machine%20Learning%20Workflow/3.3.1.feature-extraction-from-motion-data.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 3.2.2 | Seleção de _features_ com Edge Impulse | [video](https://www.youtube.com/watch?v=xQ3GBkYhXcU&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=11) [tutorial](https://docs.edgeimpulse.com/docs/tutorials/continuous-motion-recognition) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 3.2.3 | Machine learning pipeline | [video](https://www.youtube.com/watch?v=Cf1SL-EeQOQ&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=12) [slides](Module%203%20-%20Machine%20Learning%20Workflow/3.3.3.machine-learning-pipeline.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 3.2.4 | Treinamento do modelo no dge impulse | [video](https://www.youtube.com/watch?v=44v2e6JktbE&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=15) [slides](Module%203%20-%20Machine%20Learning%20Workflow/3.3.4.model-training-in-edge-impulse.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 3.2.5 | Como avaliar um model | [video](https://www.youtube.com/watch?v=jUiyXCwauJA&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=16) [slides](Module%203%20-%20Machine%20Learning%20Workflow/3.3.5.how-to-evaluate-a-model.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 3.3.6 | Underfitting e overfitting | [video](https://www.youtube.com/watch?v=6zExT6TucZg&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=17) [slides](Module%203%20-%20Machine%20Learning%20Workflow/3.3.6.underfitting-and-overfitting.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |

### Módulo 4: Implantação de modelos

Este módulo aborda as etapas para implantar um modelo de machine learning treinado no _Edge Impulse_ em uma placa Arduino. 

* Objetivos 
    - Forneça exemplos de como o aprendizado de máquina embarcado pode ser usado para resolver problemas (onde outras formas de aprendizado de máquina seriam limitadas ou inadequadas);
    - Descrever os desafios associados à execução de algoritmos de aprendizado de máquina em sistemas embarcados 
    - Descreva amplamente o que acontece durante o treinamento do modelo de aprendizado de máquina;
    - Demonstrar a capacidade de realizar inferência em um sistema embarcado para resolver um problema.



#### Microcontroladores embarcados

##### Material

| ID | Descrição | Links | Fonte |
|----|-------------|:-----:|:-----------:|
| 4.1.1 | Sistemas embarcados | [slides](Module%204%20-%20Model%20Deployment/4.2.1.embedded-systems.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 4.1.2 | Arduino Nano 33 BLE Sense | [doc](Module%204%20-%20Model%20Deployment/4.2.2.diversity-of-embedded-systems.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 4.1.3 | Hardware de computação embarcado| [slides](Module%204%20-%20Model%20Deployment/4.2.3.embedded-computing-hardware.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 4.1.4 | Microcontroladores | [doc](Module%204%20-%20Model%20Deployment/4.2.4.embedded-microcontrollers.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 4.1.5 | TinyML kit peripherals | [slides](Module%204%20-%20Model%20Deployment/4.2.6.tinyml-kit-peripherals.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 4.1.6 | Software de ML embarcados | [slides](Module%204%20-%20Model%20Deployment/4.2.8.embedded-ml-software.3.pdf?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |

#### Implantando um modelo em uma placa Arduino

##### Material

| ID | Descrição | Links | Fonte |
|----|-------------|:-----:|:-----------:|
| 4.2.1 | Usando um modelo para inferência | [video](https://www.youtube.com/watch?v=UKeZFIqMk2U&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=18) [slides](Module%204%20-%20Model%20Deployment/4.3.1.using-a-model-for-inference.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 4.2.2 | Testando inferência com um smartphone | [video](https://www.youtube.com/watch?v=OWakb-oDAOg&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=19) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 4.2.3 | Implantar modelo no Arduino | [video](https://www.youtube.com/watch?v=uUh61R8Hu0o&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG&index=20) [slides](Module%204%20-%20Model%20Deployment/4.3.3.deploy-model-to-arduino.1.pdf?raw=true) | [[1]](#1-slides-and-written-material-for-introduction-to-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 4.2.4 | Implantar modelo no Arduino | [tutorial](https://docs.edgeimpulse.com/docs/deployment/running-your-impulse-arduino) | |



### Módulo 5: Classificação de imagens com aprendizado profundo

Este módulo apresenta o conceito de classificação de imagens, por que ela é importante no aprendizado de máquina e como pode ser usada para resolver problemas. São abordadas operações de convolução e pooling, que formam os blocos de construção para redes neurais convolucionais (CNNs).

#### Classificação de imagens 

##### Material
| ID | Description | Links | Attribution |
|----|-------------|:-----:|:-----------:|
| 5.1.1 | O que é visão computacional? | [video](https://www.youtube.com/watch?v=fK8elevliKI&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=3) | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.1.2 | Visão geral das imagens digitais| [video](https://www.youtube.com/watch?v=BdLJ9Lk1I1M&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=4)  | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.1.3 | Coleta de conjunto de dados | [video](https://www.youtube.com/watch?v=uH9-Nhe8XGw&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=5) | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.1.4 | Visão geral da classificação de imagens | [video](https://www.youtube.com/watch?v=c20ditpjGjo&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=6) | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.1.5 | Treinando um classificador de imagens com Keras| [video](https://www.youtube.com/watch?v=ygzvKFgUUTA&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=8) | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |



#### Convolutional Neural Network (CNN)

##### Material

| ID | Description | Links | Attribution |
|----|-------------|:-----:|:-----------:|
| 5.2.1 | Convolução de imagem | [video](https://www.youtube.com/watch?v=glSdYcpP_v8&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=14)  | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.2.2 | Camada de pooling | [video](https://www.youtube.com/watch?v=E9TNa_6Askc&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=15)  | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.2.3 | Rede neural convolucional | [video](https://www.youtube.com/watch?v=30ikzV8Fi-0&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=16) | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.2.4 | CNN no keras | [slides](Module%206%20-%20Image%20Classification%20with%20Deep%20Learning/6.2.4.cnn-in-keras.3.pptx?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 5.2.5 | Treinando uma CNN no Edge Impulse| [video](https://www.youtube.com/watch?v=fihp_CqlcZU&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=17) [doc](Module%206%20-%20Image%20Classification%20with%20Deep%20Learning/6.2.6.training-a-cnn-in-edge-impulse.2.docx?raw=true) | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |



#### Analisando CNNs, Data Augmentation e aprendizagem por transferência (_transfer learning_)

##### Lecture Material

| ID | Description | Links | Attribution |
|----|-------------|:-----:|:-----------:|
| 5.3.1 | Visualizações da CNN | [video](https://www.youtube.com/watch?v=TmOgYgY0fTc&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=18)  | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.3.2 | Data augmentation | [video](https://www.youtube.com/watch?v=AB4dLvW5mus&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=19)  | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.3.3 | Evitando overfitting com aumento de dados | [slides](Module%206%20-%20Image%20Classification%20with%20Deep%20Learning/6.3.4.avoiding-overfitting-with-data-augmentation.3.pptx?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 5.3.4 | Explorando funções de perda e otimizadores | [doc](Module%206%20-%20Image%20Classification%20with%20Deep%20Learning/6.3.6.exploring-loss-functions-and-optimizers.3.docx?raw=true) | [[3]](#3-slides-and-written-material-for-tinyml-courseware-by-harvard-university-is-licensed-under-cc-by-nc-sa-40) |
| 5.3.5 | Transferir aprendizagem e MobileNet | [video](https://www.youtube.com/watch?v=93eczumOpx8&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=20) | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |
| 5.3.6 | Transfer learning com Edge Impulse | [video](https://www.youtube.com/watch?v=93eczumOpx8&list=PL7VEa1KauMQqQw7duQEB6GSJwDS06dtKU&index=20) [slides](Module%206%20-%20Image%20Classification%20with%20Deep%20Learning/6.3.7.transfer-learning-and-mobilenet.2.pptx?raw=true) | [[2]](#2-slides-and-written-material-for-computer-vision-with-embedded-machine-learning-by-edge-impulse-is-licensed-under-cc-by-nc-sa-40) |




### Fontes

<!-- omit in toc -->
 [1] Slides and written material for "[Introduction to Embedded Machine Learning](https://www.coursera.org/learn/introduction-to-embedded-machine-learning)" by [Edge Impulse](https://edgeimpulse.com/) is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

<!-- omit in toc -->
 [2] Slides and written material for "[Computer Vision with Embedded Machine Learning](https://www.coursera.org/learn/computer-vision-with-embedded-machine-learning)" by [Edge Impulse](https://edgeimpulse.com/) is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

<!-- omit in toc -->
 [3] Slides and written material for "[TinyML Courseware](https://github.com/tinyMLx/courseware)" by Prof. Vijay Janapa Reddi of [Harvard University](http://tinyml.seas.harvard.edu/) is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

---
<div>
  <img src="https://raw.githubusercontent.com/roscibely/algorithms-and-data-structure/develop/root/ufersa.jpg" width="900" height="250">
</div>
<i>UFERSA - Campus Pau dos Ferros</i>
