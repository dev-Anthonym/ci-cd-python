1. O que representa a etapa de CI neste projeto?
   A etapa de CI (Continuous Integration) é responsável por validar automaticamente o código sempre que ocorre uma alteração no repositório. Neste projeto,
   ela configura o ambiente Python, instala a dependências e executa os testes com o pytest. Dessa forma, é possível identificar erros antes que o código
   avance para a etapa de entrega.
   
2. O que impede a execução do Continuous Delivery quando existe um defeito?
   O que impede o Continuous Delivery é a dependência definida por "needs: ci". O Delivery só é executado quando o job de CI termina com sucesso. Quando
   um teste falha o CI fica com erro e, consequentemente, o Delivery não executado.
   
3. Qual seria a próxima etapa necessária para transformar este pipeline em Continuous Deployment?
   Seria necessário adicionar uma etapa de implantação automática (deploy) após o Delivery. Essa etapa poderia, por exemplo, enviar a aplicação para um
   servidor ou serviço de hospedagem automaticamente após a aprovação dos testes e a geração do artefato.
