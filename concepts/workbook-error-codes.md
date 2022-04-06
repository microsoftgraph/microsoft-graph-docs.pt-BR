---
title: Códigos de erro para APIs de listas de trabalho e gráficos no Microsoft Graph
description: Lista e descreve os códigos de erro e mensagens para APIs de gráficos e listas de trabalho no Microsoft Graph.
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 981be39ad78af98d131e4b38a9de49e688e27551
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672403"
---
# <a name="error-codes-for-workbooks-and-charts-apis-in-microsoft-graph"></a>Códigos de erro para APIs de listas de trabalho e gráficos no Microsoft Graph

Este artigo descreve os códigos de erro retornados pelas APIs workbooks e gráficos no Microsoft Graph quando uma solicitação enviada pela API falha. Para obter mais detalhes sobre respostas de erro e tipos de recursos no Microsoft Graph, consulte [Errors](/concepts/errors.md). Para obter detalhes sobre como lidar com respostas de Excel APIs no Microsoft Graph, consulte [Tratamento de erros](workbook-error-handling.md).

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
A seguir estão alguns códigos de erro adicionais que seu aplicativo pode encontrar no primeiro nível de objetos aninhados `innerError` . O serviço pode adicionar novos códigos de erro a qualquer momento.

- accessConflict
- accessDenied
- badRequestUncategorized
- conflictUncategorized
- filteredRangeConflict
- forbiddenUncategorized
- gatewayTimeoutUncategorized
- generalException
- insertDeleteConflict
- internalServerErrorUncategorized
- invalidArgument
- invalidReference
- invalidSessionAccessConflict
- invalidSessionAuthentication
- invalidSessionNotFound
- invalidSessionReCreatable
- invalidSessionRestricted
- invalidSessionUnexpected
- invalidSessionUnsupportedWorkbook
- itemAlreadyExists
- itemNotFound
- methodNotAllowed
- methodNotAllowedUncategorized
- nonBlankCellOffSheet
- notFoundUncategorized
- notImplementedUncategorized
- payloadTooLargeUncategorized
- rangeExceedsLimit
- requestAborted
- serviceUnavailableUncategorized
- tooManyRequestsUncategorized
- transientFailure
- unauthorizedUncategorized
- unsupportedOperation
- unsupportedWorkbook

>**Observação:** O **objeto innerError** pode conter recursivamente objetos **innerError** mais profundos com códigos de erro adicionais e mais específicos. Esses códigos **innerError** mais profundos são destinados ao desenvolvedor para ler.
<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->
