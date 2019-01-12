# Aceleração com Numba

Nesse repositório estão exemplos e dicas sobre o uso da biblioteca Numba para aceleração de scripts em Python.
Esse exemplos, em sua maioria, são baseados nos tutorais da documentação oficial do **Numba** (a qual é excelente!). Logo, os códigos aqui presentes são uma releitura com um pouco da minha experiência pessoal com o uso dos recursos da biblioteca.

**Numba** trata-se de um compilador *just-in-time* para a linguagem Python, o qual usa como base loops, arrays e funções do **NumPy**.

A sua usabilidade é bem simples e sua curva de aprendizagem pequena, pois para ativar os recursos do **Numba** basta apenas fazer de sua coleção de decoradores que ao serem aplicados em funções vão instruir como o **NUmba** deve compilá-las. A partir disso a função decorada é compilada em código de máquina, fazendo que seja notório o ganho de performace.

O **Numba** exige os seguitnes pré-requisitos:

* SO: Windows (32 e 64 bits), OSX e Linux (32 e 64 bits)
* Arquitetura: x86, x86_64, ppc64le. (Em teste: armv7l, armv8l (aarch64)).
* GPUs: Nvidia CUDA. (Em teste: AMD ROC).
* CPython
* NumPy 1.10 ou mais recente.

## Observações sobre Hardware

Os scripts deste repositório foram desenvolvidos e testados usando a seguinte configuração:

* Distribuição Anaconda (Python 3.7)
* Workstation HP 440Z
* Intel Xeon E5-1620 V3 (4 núcleos, 8 Threads, 3.5 GHz, 10 MB Cache)
* Memória RAM 16 GB 2400 MHz
* GPU Nvidia Quadro M2000

DICA: *Na ausência de hardware com GPU utilize o Google Colab!*
