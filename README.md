# Mudança de Taxa de Amostragem e Filtragem em Imagens

Este repositório contém a implementação do **Trabalho AP3** da disciplina **Processamento Digital de Sinais (PDS)**, ministrada no curso de **Engenharia de Computação** da **Universidade Federal do Ceará – Campus Sobral**.

O trabalho consiste em simulações envolvendo **mudança de taxa de amostragem**, **Transformada de Fourier bidimensional** e **filtragem de imagens**, utilizando a imagem clássica **Lenna.png**.

## 🎯 Objetivo do Trabalho

Explorar conceitos fundamentais de **Processamento Digital de Imagens**, analisando:

- Representação no domínio do espaço e da frequência
- Efeitos da subamostragem e sobreamostragem
- Fenômenos de *aliasing*
- Filtragem passa-baixa e passa-alta
- Impacto do ruído Gaussiano
- Detecção de bordas com o operador de Sobel

Todas as análises são acompanhadas de **gráficos** e **comentários explicativos diretamente no código**, conforme exigido no enunciado.

## 🧪 Atividades Implementadas

O código executa automaticamente todas as etapas abaixo:

1. Leitura da imagem **Lenna.png** e conversão para escala de cinza  
2. Cálculo e visualização do módulo e da fase da **TF bidimensional**  
3. Redução da taxa de amostragem (downsampling 3×3)  
4. Análise dos efeitos da subamostragem (*aliasing*)  
5. Aumento da taxa de amostragem (upsampling 3×3 com inserção de zeros)  
6. Análise espectral da sobreamostragem  
7. Filtragem **passa-baixa** com frequência de corte 0,1  
8. Filtragem **passa-alta** com frequência de corte 0,1  
9. Adição de **ruído Gaussiano branco** (σ = 20)  
10. Detecção de bordas com o **operador de Sobel horizontal**

Em cada etapa, o código contém comentários explicando:
- O que é observado na imagem
- Por que o comportamento ocorre

## 📌 Observações Importantes

* Não são utilizadas funções prontas para:

  * Mudança de taxa de amostragem
  * Filtragem passa-baixa ou passa-alta
* A Transformada de Fourier é:

  * Bidimensional
  * Centralizada em (0,0)
  * Visualizada em escala logarítmica (`log(1 + |FFT|)`)
