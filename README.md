# FIAP - 4° Checkpoint - IA & Machine Learning 

## Introdução
Checkpoint realizado com o intuito de colocar em prática todos os conhecimentos em Machine Learning adquiridos na matéria de IA & ML, ministrada pelo [Professor Guilherme Seidyo](https://www.linkedin.com/in/guilherme-aldeia-0a8a0b21b/).

## Participantes
- Henrique Koji
- Caio Vinicius
- Matheus Rosa
- Pedro Augusto

## Notebooks

Há três notebooks desenvolvidos para aprofundar o entendimento sobre modelos de linguagem. 

1.  O primeiro foca no entendimento de LLMs (Large Language Models), abordando conceitos básicos e arquiteturas utilizadas.
2.  O segundo explora o funcionamento de tokens e as diferenças entre diversos modelos de linguagem, ajudando a entender como eles processam e geram texto. 
3.  O terceiro notebook é um desafio proposto pelo professor, onde os alunos devem aplicar os conhecimentos adquiridos para resolver um problema prático relacionado ao uso de modelos de linguagem.

## Desafio
O desafio consiste em desenvolver um programa que receba um prompt e utilize o [Jailbreak Classifier](https://huggingface.co/jackhhao/jailbreak-classifier) para verificar se há a presença de um jailbreak. Após fazer a validação de jailbreak do prompt utlizar o LLM [TinyLlama-1.1B-Chat-v1.0](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0) para gerar o resto do prompt. A proposta envolve o uso dessa ferramenta para analisar entradas de texto e identificar qualquer tentativa de contornar restrições de modelos de linguagem ou outros sistemas de segurança.

## O que é Jailbreak
Jailbreak é um termo usado para descrever o processo de remover restrições impostas por fabricantes de software ou dispositivos, permitindo que os usuários acessem funcionalidades ou executem códigos que normalmente seriam bloqueados. Em modelos de linguagem e sistemas de IA, o jailbreak refere-se a técnicas que exploram vulnerabilidades para obter respostas que violam as diretrizes de uso, como a geração de conteúdo inapropriado, enviesado ou que infringe políticas de segurança e ética.

## O que é fine-tunning
O ajuste fino (ou fine-tuning em inglés) é uma técnica de treinamento que consiste na reutilização de arquiteturas de CNN (rede neural convolucional) predefinidas e pré-treinadas. Basicamente, permite que você pegue um modelo treinado que executa bem uma determinada tarefa e aproveite todo o seu conhecimento para resolver uma nova tarefa específica; embora, é claro, seguindo determinadas regras.

## Como a combinação de duas LLMs pode ser feita para melhorar a segurança de uso?
1. Duas LLMs podem ser usadas em conjunto para validar as respostas uma da outra. Se uma LLM gerar uma resposta, a outra pode verificar se essa resposta atende a critérios de segurança. 

2. As LLMs podem ser treinadas ou ajustadas para funções específicas. Por exemplo, uma LLM pode se especializar na detecção de conteúdo malicioso, enquanto a outra se foca na geração de respostas apropriadas

3. Ao usar duas LLMs diferentes, pode mitigar o risco de um ataque jailbreak funcionar. Mesmo que um atacante consiga enganar a primeira LLM para gerar uma resposta inadequada, a segunda LLM pode servir como uma barreira adicional e um segundo checker. Só ai, o prompt seria gerado.
