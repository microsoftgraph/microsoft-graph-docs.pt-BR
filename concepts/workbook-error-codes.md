---
title: Códigos de erro para APIs de listas de trabalho e gráficos no Microsoft Graph
description: Lista e descreve os códigos de erro e mensagens para APIs de gráficos e listas de trabalho no Microsoft Graph.
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 43aeb851cd5f458c2dda971938e0d0b6fa193c85d35ba0bac54edbc904acf964
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54225584"
---
# <a name="error-codes-for-workbooks-and-charts-apis-in-microsoft-graph"></a>Códigos de erro para APIs de listas de trabalho e gráficos no Microsoft Graph

Este artigo descreve os códigos de erro retornados pelas APIs workbooks e gráficos no Microsoft Graph quando uma solicitação enviada pela API falha. Para obter mais detalhes sobre respostas de erro e tipos de recursos no Microsoft Graph, consulte [Errors](/concepts/errors.md).

## <a name="error-code"></a>Código de erro

A tabela a seguir lista os códigos de erro e as mensagens atuais. O serviço pode adicionar novos códigos de erro a qualquer momento. 

| Código de Status               | Código do erro                       | Mensagem de erro
|:--------------------------|:--------------------------|:--------------
|400    | **badRequest**          | A solicitação está incorreta ou foi mal formada.
|401    | **não autorizado**  | O chamador não está autenticado.
|403    | **forbidden**      | O chamador não tem permissão para executar a ação.
|404    | **notFound**          | Não foi possível localizar o recurso.
|405    | **methodNotAllowed**        | O método HTTP na solicitação não é permitido no recurso.
|409    | **conflict**          | O estado atual está em conflito com o que a solicitação espera.
|413    | **payloadTooLarge**       | O tamanho da solicitação excede o limite máximo.
|429    | **tooManyRequests**     | O aplicativo ou o usuário foi restringido.
|500    | **internalServerError**            | Ocorreu um erro de servidor interno durante o processamento da solicitação.
|501    | **notImplemented**          | O recurso solicitado não foi implementado.
|502    | **badGateway**          | O servidor encontrou um erro temporário e não pôde concluir sua solicitação.
|503    | **serviceUnavailable**      | O serviço não está disponível. Tente sua solicitação novamente.
|504    | **gatewayTimeout**        | O servidor, ao atuar como proxy, não recebeu uma resposta em tempo há tempo do servidor upstream para concluir a solicitação.

## <a name="detailed-error-code"></a>Código de erro detalhado
A seguir estão alguns erros adicionais que seu aplicativo pode encontrar no primeiro nível de objetos `innerError` aninhados. O serviço pode adicionar novos códigos de erro a qualquer momento.

| Código                               | Mensagem
|:-----------------------------------|:----------------------------------------------------------
| **accessConflict**   |A solicitação falhou devido a conflitos com outros clientes que estão acessando a workbook.
| **accessDenied**         | Você não pode realizar a operação solicitada.
| **badRequestUncategorized**               | A solicitação está incorreta ou foi mal formada.
| **conflictUncategorized**                   | O estado atual está em conflito com o que a solicitação espera.
| **filteredRangeConflict**                   | A operação falhou porque entra em conflito com um intervalo filtrado.
| **forbiddenUncategorized**                    | A solicitação não é permitida.
| **gatewayTimeoutUncategorized**         | O serviço não pôde concluir a solicitação dentro do limite de tempo.
| **generalException**         | Ocorreu um erro interno ao processar a solicitação.
| **insertDeleteConflict**         | A tentativa de operação de exclusão ou inserção resultou em um conflito.
| **internalServerErrorUncategorized**       | Ocorreu um erro não especificado.
| **invalidArgument**         | O argumento é inválido, está ausente ou tem um formato incorreto.
| **invalidReference**         | Esta referência não é válida para a operação atual.
| **invalidSessionAccessConflict**             | A sessão especificada na solicitação é inválida devido a conflitos com outros clientes que estão acessando a workbook.
| **invalidSessionAuthentication**         | A sessão especificada na solicitação é inválida devido a um erro de autenticação.
| **invalidSessionNotFound**         | A sessão especificada na solicitação é inválida porque a workbook não pode ser encontrada.
| **invalidSessionReCreatable**             | A sessão especificada na solicitação não existe ou é inválida devido a um erro transitório.
| **invalidSessionRestricted**          | A sessão especificada na solicitação é inválida devido a configurações de serviço ou restrições.
| **invalidSessionUnexpected**                | A sessão especificada na solicitação é inválida devido a um problema inesperado.
| **invalidSessionUnsupportedWorkbook**              | A sessão especificada na solicitação é inválida porque a workbook contém recursos não compatíveis ou excede o limite de tamanho.
| **itemAlreadyExists**         | O recurso que está sendo criado já existe.
| **itemNotFound**         | O recurso solicitado não existe.
| **methodNotAllowed**              | O método HTTP especificado na solicitação não é permitido no recurso.
| **methodNotAllowedUncategorized**              | O método HTTP especificado na solicitação não é permitido no recurso.
| **nonBlankCellOffSheet**         | Não é possível inserir novas células porque ela empurraria células não vazias para fora do final da planilha.
| **notFoundUncategorized**             | O recurso solicitado não pode ser encontrado.
| **notImplementedUncategorized**            | O recurso solicitado não está implementado no momento.
| **payloadTooLargeUncategorized**              | A carga de solicitação excede o limite de tamanho.
| **rangeExceedsLimit**         | A contagem de células no intervalo excedeu o número máximo suportado.
| **requestAborted**         | A solicitação foi anulada durante o tempo de execução.
| **serviceUnavailableUncategorized**      | O serviço está temporariamente indisponível ou está sobrecarregado. Tente sua solicitação novamente.
| **tooManyRequestsUncategorized**             | O aplicativo cliente ou o usuário foi desacelerado. Tente sua solicitação novamente.
| **transientFailure**           | A solicitação falhou devido a um erro transitório. Tente sua solicitação novamente.
| **unauthorizedUncategorized**         | As informações de autenticação necessárias para o recurso estão ausentes ou inválidas.
| **unsupportedOperation**         | Não há suporte para a operação que está sendo tentada.
| **unsupportedWorkbook**         | A solicitação falhou. A workbook contém recursos sem suporte ou excede o limite de tamanho.

>**Observação:** O **objeto innerError** pode conter recursivamente objetos **innerError** mais profundos com códigos de erro adicionais e mais específicos. Esses códigos **innerError** mais profundos são destinados ao desenvolvedor para ler.
<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->
