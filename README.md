⚙️ Escalonamento de Processos — FCFS, Round Robin e SJF

📌 Sobre o projeto

Este repositório contém uma atividade prática de Sistemas Operacionais, desenvolvida em Python utilizando Jupyter Notebook.

O projeto tem como objetivo simular e comparar diferentes algoritmos de escalonamento de processos, analisando como cada política influencia a ordem de execução, o tempo de espera e o tempo de conclusão dos processos.

A implementação foi baseada no material disponibilizado pelo professor, com adaptações para atender ao desafio proposto.

🎯 Objetivos

* Implementar e comparar os algoritmos FCFS, Round Robin e SJF.
* Adicionar o processo P4, com tempo de chegada 3 e burst 1.
* Simular Round Robin com quantums de 1, 2 e 4 unidades de tempo.
* Identificar qual política de escalonamento favorece o processo P4.
* Representar visualmente a execução por meio de gráficos de Gantt.

🧠 Algoritmos utilizados

FCFS — First Come, First Served

Executa os processos de acordo com a ordem de chegada. É um algoritmo simples e não preemptivo, mas pode provocar longos tempos de espera.

Round Robin — RR

Distribui o tempo da CPU entre os processos utilizando um quantum definido.

Foram utilizados três valores de quantum:

* q = 1
* q = 2
* q = 4

O objetivo é observar como a duração do quantum influencia o tempo de conclusão dos processos.

SJF — Shortest Job First

Seleciona, entre os processos disponíveis, aquele que possui o menor tempo de execução (burst).

Nesta atividade, foi implementada a versão não preemptiva, em que o processo selecionado executa até terminar.

📊 Análise dos resultados

A comparação considera o processo P4, configurado com:

Processo	Chegada	Burst
P4	3	1

Os resultados obtidos na simulação foram:

Algoritmo	Conclusão de P4	Tempo de espera
FCFS	13	9
Round Robin (q=1)	6	2
Round Robin (q=2)	9	5
Round Robin (q=4)	11	7
SJF	7	3

O Round Robin com quantum 1 apresentou o melhor resultado para P4, permitindo que o processo fosse concluído mais rapidamente.

Os gráficos de Gantt disponíveis no notebook permitem visualizar as diferenças entre as políticas.

🚀 Como executar

1. Acesse o Google Colab.
2. Faça o upload do arquivo Atividade_7_Agendamento_Processos.ipynb.
3. Selecione Ambiente de execução → Executar tudo.
4. Aguarde a execução das células.
5. Analise os resultados e os gráficos de Gantt gerados.

Tecnologias utilizadas: Python 3, Jupyter Notebook, Google Colab e Matplotlib.

📚 Referência

Atividade desenvolvida com base no notebook disponibilizado pelo professor:

Material original — Agendamento de Processos

👨‍💻 Autor

Matheus Gonzalez Tendulini

Engenharia da Computação

⸻

Projeto desenvolvido para fins acadêmicos, com foco no estudo e na comparação de algoritmos de escalonamento de processos.