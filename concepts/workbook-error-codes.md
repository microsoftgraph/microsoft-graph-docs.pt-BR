---
title: Códigos de erro para APIs de planilhas e gráficos no Microsoft Graph
description: Lista e descreve os códigos de erro e as mensagens de pastas de trabalho e de gráficos no Microsoft Graph.
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 92c5512d20f6d93efefa00a1e3fa55bf0c8a82d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018092"
---
# <a name="error-codes-for-workbooks-and-charts-apis-in-microsoft-graph"></a>Códigos de erro para APIs de planilhas e gráficos no Microsoft Graph

Este artigo descreve os códigos de erro que são retornados pelas APIs de planilhas e gráficos no Microsoft Graph quando uma solicitação enviada por meio da API falha. Para obter mais detalhes sobre respostas de erro e tipos de recurso no Microsoft Graph, confira [erros](/concepts/errors.md).

## <a name="error-code"></a>Código de erro

A tabela a seguir lista os códigos de erro e mensagens atuais. O serviço pode adicionar novos códigos de erro a qualquer momento. 

| Código de status               | Código do erro                       | Mensagem de erro
|:--------------------------|:--------------------------|:--------------
|400    | **badRequest**          | A solicitação está incorreta ou foi mal formada.
|401    | **não autorizado**  | O chamador não está autenticado.
|403    | **proibido**      | O chamador não tem permissão para executar a ação.
|404    | **não encontrado**          | Não foi possível localizar o recurso.
|405    | **methodNotAllowed**        | O método HTTP na solicitação não é permitido no recurso.
|409    | **apresentar**          | O estado atual está em conflito com o que a solicitação espera.
|413    | **payloadTooLarge**       | O tamanho da solicitação excede o limite máximo.
|429    | **tooManyRequests**     | O aplicativo ou o usuário foi restringido.
|500    | **internalServerError**            | Ocorreu um erro interno no servidor ao processar a solicitação.
|501    | **notImplemented**          | O recurso solicitado não foi implementado.
|502    | **badGateway**          | O servidor encontrou um erro temporário e não pôde concluir sua solicitação.
|503    | **serviceUnavailable**      | O serviço não está disponível. Tente a solicitação novamente.
|504    | **gatewayTimeout**        | O servidor, ao atuar como um proxy, não recebeu uma resposta em tempo hábil do servidor upstream para concluir a solicitação.

## <a name="detailed-error-code"></a>Código de erro Detalhado
A seguir estão alguns erros adicionais que seu aplicativo pode encontrar no primeiro nível de objetos aninhados `innerError` . O serviço pode adicionar novos códigos de erro a qualquer momento.

| Código                               | Mensagem
|:-----------------------------------|:----------------------------------------------------------
| **accessConflict**   |A solicitação falhou devido a conflitos com outros clientes que estão acessando a pasta de trabalho.
| **accessDenied**         | Você não pode realizar a operação solicitada.
| **badRequestUncategorized**               | A solicitação está incorreta ou foi mal formada.
| **conflictUncategorized**                   | O estado atual está em conflito com o que a solicitação espera.
| **filteredRangeConflict**                   | A operação falhou porque está em conflito com um intervalo filtrado.
| **forbiddenUncategorized**                    | A solicitação não é permitida.
| **gatewayTimeoutUncategorized**         | O serviço não pôde concluir a solicitação dentro do limite de tempo.
| **generalException**         | Ocorreu um erro interno ao processar a solicitação.
| **insertDeleteConflict**         | A tentativa de operação de exclusão ou inserção resultou em um conflito.
| **internalServerErrorUncategorized**       | Ocorreu um erro não especificado.
| **invalidArgument**         | O argumento é inválido, está ausente ou tem um formato incorreto.
| **invalidReference**         | Esta referência não é válida para a operação atual.
| **invalidSessionAccessConflict**             | A sessão especificada na solicitação é inválida devido a conflitos com outros clientes que estão acessando a pasta de trabalho.
| **invalidSessionAuthentication**         | A sessão especificada na solicitação é inválida devido a um erro de autenticação.
| **invalidSessionNotFound**         | A sessão especificada na solicitação é inválida porque a pasta de trabalho não pode ser encontrada.
| **invalidSessionReCreatable**             | A sessão especificada na solicitação não existe ou é inválida devido a um erro transitório.
| **invalidSessionRestricted**          | A sessão especificada na solicitação é inválida devido a configurações ou restrições de serviço.
| **invalidSessionUnexpected**                | A sessão especificada na solicitação é inválida devido a um problema inesperado.
| **invalidSessionUnsupportedWorkbook**              | A sessão especificada na solicitação é inválida porque a pasta de trabalho contém recursos sem suporte ou excede o limite de tamanho.
| **itemAlreadyExists**         | O recurso que está sendo criado já existe.
| **itemNotFound**         | O recurso solicitado não existe.
| **methodNotAllowed**              | O método HTTP especificado na solicitação não é permitido no recurso.
| **methodNotAllowedUncategorized**              | O método HTTP especificado na solicitação não é permitido no recurso.
| **nonBlankCellOffSheet**         | Não é possível inserir novas células porque elas empurraram células não vazias para fora do final da planilha.
| **notFoundUncategorized**             | O recurso solicitado não pode ser encontrado.
| **notImplementedUncategorized**            | O recurso solicitado não foi implementado no momento.
| **payloadTooLargeUncategorized**              | A carga de solicitação excede o limite de tamanho.
| **rangeExceedsLimit**         | A contagem de células no intervalo excedeu o número máximo com suporte.
| **requestAborted**         | A solicitação foi anulada durante o tempo de execução.
| **serviceUnavailableUncategorized**      | O serviço está temporariamente indisponível ou está sobrecarregado. Tente a solicitação novamente.
| **tooManyRequestsUncategorized**             | O usuário ou aplicativo cliente foi limitado. Tente a solicitação novamente.
| **transientFailure**           | A solicitação falhou devido a um erro transitório. Tente a solicitação novamente.
| **unauthorizedUncategorized**         | As informações de autenticação necessárias para o recurso estão ausentes ou são inválidas.
| **unsupportedOperation**         | Não há suporte para a operação que está sendo tentada.
| **unsupportedWorkbook**         | A solicitação falhou. A pasta de trabalho contém recursos sem suporte ou excede o limite de tamanho.

>**Observação:** O objeto **innerError** pode conter recursivamente objetos de **innerError** mais profundos com códigos de erro adicionais e mais específicos. Esses códigos **innerError** mais profundos são intendad para que o desenvolvedor Leia.
<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->
