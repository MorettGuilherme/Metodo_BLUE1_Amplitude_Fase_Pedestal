A primeira versão do método Melhor Estimador Linear Não Enviesado (Best Linear Blue Estimador - BLUE 1) tem o objetivo de encontrar um vetor de parâmetros estimados, cujos componentes são respectivamente: amplitude, amplitude vezes fase e pedestal.
Obs.: nesse algoritmo, a fase estimada é calculada pela divisão entre o termo da amplitude versus a fase pela amplitude estimada.

Nesse repositório, o algoritmo foi desenvolvido para o cálculo individual do erro de estimação desses parâmetros pela técnica de validação cruzada K-Fold.

Comentários sobre os resultados: de acordo com a análise estatística notou-se que não há um janelamento ideal para amplitude visto que o desvio padrão não se estabiliza para um certo valor de janelamento adotado. Portanto, o último janelamento a ser analizado 19 foi considerado como o ideal.
Ademais para a fase, os resultados não foram satisfatórios, devido ao fato da dispersão dos dados em relação a média serem elevados. Portanto, novas estrátegias para o cálculo da fase devem ser avaliadas. O que foi proposto é adotar um valor mínimo para a amplitude estimada. Outra alternativa é calcular a fase estimada por meio da amplitude de referência.

A seguir são listadas as pastas e também os arquivos contidos nesse repositório, assim como suas respectivas funções:

1. Dados_Estatisticos_BLUE1_amplitude_OC
  * Essa pasta contém arquivos para cada um dos janelamentos com os valores das ocupações e médias, variâncias e desvios padrão associados para o erro de estimação da amplitude.

2. Dados_Estatisticos_BLUE1_fase_amplitude_estimada_OC
  * Essa pasta contém arquivos para cada um dos janelamentos com os valores das ocupações e médias, variâncias e desvios padrão associados para o erro de estimação da fase, por meio da amplitude estimada.

3. Dados_Estatisticos_BLUE1_fase_amplitude_referencia_OC
  * Essa pasta contém arquivos para cada um dos janelamentos com os valores das ocupações e médias, variâncias e desvios padrão associados para o erro de estimação da fase, por meio da amplitude de referência.
  
4. Dados_Estatisticos_BLUE1_pedestal_OC
  * Essa pasta contém arquivos para cada um dos janelamento com os valores das ocupações e médias, variâncias e desvios padrão associados para o erro de estimação do pedestal.

5. Dados_Ocupacoes_Free_Running
  * Essa pasta contém arquivos com os dados para cada uma das ocupações referentes ao pulso de sinal, amplitude de referência, fase de referência e ruído eletrônico registrados a cada 25 ns.
  
6. K_Fold_amplitude_DP_Dados_Estatisticos_BLUE1_OC
  * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão dos desvios padrão dos erros de estimação da amplitude calculados pela técnica de validação cruzada K-Fold.

7. K_Fold_amplitude_DP_Desempenho_BLUE1_OC
  * Essa pasta contém um arquivo com os dados da análise estatística do desvio padrão do erro de estimação da amplitude para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

8. K_Fold_amplitude_EME_Desempenho_BLUE1_OC
  * Essa pasta contém um arquivo com os dados da análise do erro médio de estimação (EME) da amplitude para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

9. K_Fold_amplitude_MAE_Desempenho_BLUE1_OC
  * Essa pasta contém um arquivo com os dados da análise do erro médio absoluto (MAE) da amplitude para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold.

10. K_Fold_amplitude_media_Dados_Estatisticos_BLUE1_OC
  * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão das médias dos erros de estimação da amplitude calculados pela técnica de validação cruzada K-Fold.

11. K_Fold_amplitude_MSE_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise do erro médio quadrático (MSE) da amplitude para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

12. K_Fold_amplitude_SNR_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise da relação sinal ruído (SNR) da amplitude para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

13. K_Fold_amplitude_var_Dados_Estatisticos_BLUE1_OC
  * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão das variâncias dos erros de estimação da amplitude calculados pela técnica de validação cruzada K-Fold.

14. K_Fold_fase_amplitude_estimada_DP_Dados_Estatisticos_BLUE1_OC
  * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão dos desvios padrão dos erros de estimação da fase pela amplitude estimada calculados pela técnica de validação cruzada K-Fold.

15. K_Fold_fase_amplitude_estimada_DP_Desempenho_BLUE1_OC
  * Essa pasta contém um arquivo dos dados estatísticos para cada ocupação do desvio padrão para o erro de estimação da fase, por meio da amplitude estimada.

16. K_Fold_fase_amplitude_estimada_EME_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise do erro médio de estimação (EME) da fase pela amplitude estimada para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

17. K_Fold_fase_amplitude_estimada_MAE_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise do erro médio absoluto (MAE) da fase pela amplitude estimada para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

18. K_Fold_fase_amplitude_estimada_media_Dados_Estatisticos_BLUE1_OC
   * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão das médias dos erros de estimação da fase pela amplitude estimada calculados pela técnica de validação cruzada K-Fold.

19. K_Fold_fase_amplitude_estimada_MSE_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise do erro médio quadrático (MSE) da fase pela amplitude estimada para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

20. K_Fold_fase_amplitude_estimada_SNR_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise da relação sinal ruído (SNR) da fase pela amplitude estimada para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

21. K_Fold_fase_amplitude_estimada_var_Dados_Estatisticos_BLUE1_OC
   * Essa pasta contém arquivos para cada uma das ocupações dos dados estatísticos da variância do erro de estimação da fase pela amplitude estimada.

22. K_Fold_fase_amplitude_referencia_DP_Dados_Estatisticos_BLUE1_OC
  * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão dos desvios padrão dos erros de estimação da fase pela amplitude de referência calculados pela técnica de validação cruzada K-Fold.

23. K_Fold_fase_amplitude_referencia_DP_Desempenho_BLUE1_OC
  * Essa pasta contém um arquivo dos dados estatísticos para cada ocupação do desvio padrão para o erro de estimação da fase, por meio da amplitude de referência.

24. K_Fold_fase_amplitude_referencia_EME_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise do erro médio de estimação (EME) da fase pela amplitude de referência para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

25. K_Fold_fase_amplitude_referencia_MAE_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise do erro médio absoluto (MAE) da fase pela amplitude de referência para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

26. K_Fold_fase_amplitude_referencia_media_Dados_Estatisticos_BLUE1_OC
   * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão das médias dos erros de estimação da fase pela amplitude de referência calculados pela técnica de validação cruzada K-Fold.

27. K_Fold_fase_amplitude_referencia_MSE_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise do erro médio quadrático (MSE) da fase pela amplitude de referência para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

28. K_Fold_fase_amplitude_referencia_SNR_Desempenho_BLUE1_OC
   * Essa pasta contém um arquivo com os dados da análise da relação sinal ruído (SNR) da fase pela amplitude de referência para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold para todas as ocupações.

29. K_Fold_fase_amplitude_referencia_var_Dados_Estatisticos_BLUE1_OC
   * Essa pasta contém arquivos para cada uma das ocupações dos dados estatísticos da variância do erro de estimação da fase pela amplitude de referência.

30. K_Fold_fase_analise_amplitude_minima_estimada_DP_J_19
  * Essa pasta contém os arquivos da análise do desvio padrão do erro de estimação da fase pela amplitude mínima estimada pelo K-Fold das ocupações 10 a 100.

31. K_Fold_fase_analise_amplitude_minima_estimada_media_J_19
  * Essa pasta contém os arquivos da análise da média do erro de estimação da fase pela amplitude mínima estimada pelo K-Fold das ocupações 10 a 100.

32. K_Fold_fase_analise_amplitude_minima_estimada_var_J_19
  * Essa pasta contém os arquivos da análise da variância do erro de estimação da fase pela amplitude mínima estimada pelo K-Fold das ocupações 10 a 100.

33. K_Fold_fase_analise_amplitude_minima_referencia_DP_J_19
  * Essa pasta contém os arquivos da análise do desvio padrão do erro de estimação da fase pela amplitude mínima de referência pelo K-Fold das ocupações 10 a 100.

34. K_Fold_fase_analise_amplitude_minima_referencia_media_J_19
  * Essa pasta contém os arquivos da análise da média do erro de estimação da fase pela amplitude mínima de referencia pelo K-Fold das ocupações 10 a 100.

35. K_Fold_fase_analise_amplitude_minima_referencia_var_J_19
  * Essa pasta contém os arquivos da análise da variância do erro de estimação da fase pela amplitude mínima de referência pelo K-Fold das ocupações 10 a 100.

36. K_Fold_pedestal_DP_Dados_Estatisticos_BLUE1_OC
   * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão dos desvios padrão dos erros de estimação do pedestal calculados pela técnica de validação cruzada K-Fold.

37. K_Fold_pedestal_DP_Desempenho_BLUE1_OC
   * Essa pasta contém arquivos com os dados da análise do desvio padrão do erro estimação para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold.

38. K_Fold_pedestal_EME_Desempenho_BLUE1_OC
   * Essa pasta contém arquivos com os dados da análise do erro médio de estimação (EME) para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold.

39. K_Fold_pedestal_MAE_Desempenho_BLUE1_OC
   * Essa pasta contém arquivos com os dados da análise do erro médio absoluto (MAE) para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold.

40.  K_Fold_pedestal_media_Dados_Estatisticos_BLUE1_OC
   * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão das médias dos erros de estimação do pedestal calculados pela técnica de validação cruzada K-Fold.

41. K_Fold_pedestal_MSE_Desempenho_BLUE1_OC
   * Essa pasta contém arquivos com os dados da análise do erro médio quadrático (MSE) para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold.

42. K_Fold_pedestal_SNR_Desempenho_BLUE1_OC
   * Essa pasta contém arquivos com os dados da análise da relação sinal ruído (SNR) para o janelamento ideal 19 calculados pela técnica de validação cruzada K-Fold.

43. K_Fold_pedestal_var_Dados_Estatisticos_BLUE1_OC
   * Essa pasta contém arquivos para cada uma das ocupações; os valores dos janelamentos com as médias, variâncias e desvios padrão das médias dos erros de estimação do pedestal calculados pela técnica de validação cruzada K-Fold.

44. Resultados_BLUE1_Amplitude
   * Essa pasta com os gráficos dos dados estatísticos (média, variância e desvio padrão) para o erro de estimação da amplitude pela técnica da validação cruzada K-Fold, assim como os histogramas para cada janelamento e ocupações e a análise do desempenho.

45. Resultados_BLUE1_Fase_amplitude_Estimada
   * Essa pasta com os gráficos dos dados estatísticos (média, variância e desvio padrão) para o erro de estimação da fase pela amplitude estimada pela técnica da validação cruzada K-Fold, assim como os histogramas para cada janelamento e ocupações e a análise do desempenho.

46. Resultados_BLUE1_Fase_amplitude_Referencia
   * Essa pasta com os gráficos dos dados estatísticos (média, variância e desvio padrão) para o erro de estimação da fase pela amplitude de referência pela técnica da validação cruzada K-Fold, assim como os histogramas para cada janelamento e ocupações e a análise do desempenho.
   
47. Resultados_BLUE1_Pedestal
   * Essa pasta com os gráficos dos dados estatísticos (média, variância e desvio padrão) para o erro de estimação do pedestal pela técnica da validação cruzada K-Fold, assim como os histogramas para cada janelamento e ocupações e a análise do desempenho.

48. arquivo_saida_analise_amplitude_minima_fase_BLUE1.py
   * Instrução para salvar em arquivos os dados estatísticos pela validação cruzada k-Fold para a estimação da fase.
   * Instrução da validação cruzada K-Fold para a análise de como o valor da amplitude mínima adotado influencia no processo de estimação da fase.
   * Instrução principal.

49. arquivo_saida_dados_estatisticos_BLUE1.py
   * Função para o cálculo dos dados estatísticos do erro de estimação pelo método Best Linear Unbiased Estimator (BLUE 1).
   * Instrução para salvar os dados estatísticos do erro de estimação da amplitude, fase ou pedestal para determinada ocupação em um arquivo de saída.
   * Instrução principal do código.

50. arquivo_saida_desempenho_BLUE1.py
   * Instrução para salvar em arquivos os dados estatísticos do desempenho do método BLUE 1.
   * Função para o cálculo do desempenho do método BLUE 1 pelo Erro Médio de Estimação (EME).
   * Função para o cálculo do desempenho do método BLUE 1 pelo Erro Médio Quadrático (Mean Squared Error - MSE).
   * Função para o cálculo do desempenho do método BLUE 1 pelo Erro Médio Absoluto (Mean Absolute Error - MAE).
   * Função para o cálculo do desempenho do método BLUE 1 pela Relação Sinal-Ruído (Signal-to-Noise Ratio - SNR).
   * Função para o cálculo do desempenho do método BLUE 1 pelo desvio padrão (DP).
   * Instrução da validação cruzada K-Fold adaptada para o cálculo do desempenho do método BLUE 1.
   * Instrução principal do código.

51. arquivo_saida_k_fold_BLUE1.py
   * Instrução para salvar em arquivos os dados estatísticos pela validação cruzada k-Fold.
   * Instrução da validação cruzada K-Fold.
   * Instrução principal do código.

52. grafico_analise_amplitude_minima_fase_BLUE1.py
   * Função para a leitura dos dados estatísticos da análise erro de estimação da fase para uma dada ocupação pelo método BLUE1.
   * Instrução para o plote do gráfico do dado estatístico ao longo das ocupações para um determinado janelamento pelo processo de estimação da fase.
   * Instrução principal do código.
   
53. grafico_dado_estatistico_janelamento_BLUE1.py
   * Função para a leitura dos dados estatísticos de todas as ocupações para um determinado janelamento.
   * Instrução para o plote do gráfico do dado estatístico ao longo das ocupações para um determinado janelamento.
   * Instrução principal do código.

54. grafico_desempenho_BLUE1.py
   * Função para a leitura dos dados do desempenho do método BLUE 1 de todas as ocupações para o janelamento ideal.
   * Instrução para o plote do gráfico do desempenho do método BLUE 1 ao longo das ocupações para o janelamento ideal.
   * Instrução principal do código.

55. grafico_k_fold_BLUE1.py
   * Função para a leitura dos dados estatísticos da validação cruzada K-Fold.
   * Instrução para a construção do gráfico tipo A da validação cruzada K-Fold.
   * Instrução para a construção do gráfico tipo B da validação cruzada K-Fold.
   * Instrução principal (main) do código.
   
56. histograma_erro_parametro_BLUE1.py
   * Função para o cálculo da estatística do erro de estimação da amplitude, fase ou pedestal.
   * Instrução para o plote do histograma do tipo A do erro de estimação da amplitude, fase ou pedestal.
   * Instrução para o plote do histograma do tipo B do erro de estimação da amplitude, fase ou pedestal.
   * Instrução principal (main) do código.
   
57. leitura_dados_ocupacao_BLUE1.py
   * Função para a leitura dos dados de ocupação.
   * Função para a retirada do pedestal dos pulsos de sinais.
   * Função para a construção da matriz dos pulsos de sinais e o vetor do parâmetro de referência.
   * Função para separação em dados de treino e teste.

58. leitura_dados_ruidos_BLUE1.py
   * Função para a leitura dos dados de ruídos de acordo com a ocupação.
   * Função para a organização dos dados de ruídos de acordo com o janelamento.
   * Função para separação em dados de treino e teste.
   * Função para a construção da matriz de covariância.
   * Função para a construção da matriz de covariância como identidade.

59. metodo_BLUE1.py
   * Função para a definição do vetor pulso de referência.
   * Função para a definição do vetor da derivada temporal do pulso de referência.
   * Função para o método BLUE 1.
   
IMPORTANTE: os dados das ocupações foram simulados computacionalmente. As características das distribuições são:

* Distribuição amplitude: exponencial com média 100 ADC Count.
* Distribuição Fase: uniforme com números inteiros no intervalo de -5 a 5 ns.
* Pedestal: 30 ADC Count.
* Nível de deformação: 0,01 ADC Count.
* Número de eventos: 2000000.
* Fold: 100.
* Os dados de ruídos para a matriz de covariância foram os mesmos que para os pulsos de sinais.

Obs.: antes da aplicação do método, o valor constante do pedestal foi retirado dos dados referentes aos pulsos de sinais.
O vetor da fase de referência foi multiplicado por 0,5; pois esse valor representa a resolução da fase.
