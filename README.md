# DSBD
Repositório para a Disciplina de Infraestrutura Computacional - Especialização Data Science e Big Data UFPR:

Este é um script para baixar dados de despesas no site da transparência.
Os comandosforam utilizados a partir da seguinte lógica:

 Define um código BASH
 Ativa o modo de debug (exibir cada comando e mostrando outros detalhes)
 Indica qual o endereço do site
 Variáveis indicando os dias do mês da busca, o mês e o ano que irá buscar
 Diretórios que serão utilizados para baixar os dados e processá-los
 Cria diretorio
 Define o primeiro arquivo do diretorio 
 Executa o for para cada dia (inicio e fim) do período
 O comando wget vai baixar o arquivo zip com os dados do site 
 dados são descompactados no diretório temporário
 Arquivo zip é removido
 Condiciona qual o arquivo para manter ou excluir o cabeçalho
 Dados são copiados do diretório temporário para o diretório dados adicionando o novo arquivo no final do anterior
 Repete o processo para o outro arquivo
 Diretório temporário é apagado

 [IMPORTANTE]
 Garantir que o diretório em que o arquivo "baixaDadosTransp.sh" está exista.
 Conferir as permissões para executar no diretório
 Passar os parâmetros corretamente