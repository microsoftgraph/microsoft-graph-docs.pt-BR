---
title: Códigos de erro para APIs de pastas de trabalho e gráficos
description: Lista e descreve os códigos de erro retornados pelas APIs de pastas de trabalho e gráficos no Microsoft Graph quando uma solicitação enviada por meio da API falha.
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 88921271f38f9ae8ad440ea40a2733b890e14d83
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444177"
---
# <a name="error-codes-for-workbooks-and-charts-apis"></a>Códigos de erro para APIs de pastas de trabalho e gráficos

Este artigo descreve os códigos de erro retornados pelas APIs de pastas de trabalho e gráficos no Microsoft Graph quando uma solicitação enviada por meio da API falha. Para obter mais detalhes sobre respostas de erro e tipos de recursos no Microsoft Graph, consulte [Erros](/concepts/errors.md). Para obter detalhes sobre como lidar com respostas de erro de APIs do Excel no Microsoft Graph, consulte [Tratamento de erros](workbook-error-handling.md).

## <a name="error-codes-and-messages"></a>Códigos de erro e mensagens

A tabela a seguir lista os códigos de erro e as mensagens atuais. O serviço pode adicionar novos códigos de erro a qualquer momento.

| Código de status | Código de erro                | Mensagem de erro
|:------------|:--------------------------|:--------------
|400          | **badRequest**            | A solicitação está incorreta ou foi mal formada.
|401          | **Desautorizado**          | O chamador não está autenticado.
|403          | **Proibido**             | O chamador não tem permissão para executar a ação.
|404          | **Notfound**              | Não foi possível localizar o recurso.
|405          | **methodNotAllowed**      | O método HTTP na solicitação não é permitido no recurso.
|409          | **Conflito**              | O estado atual está em conflito com o que a solicitação espera.
|413          | **payloadTooLarge**       | O tamanho da solicitação excede o limite máximo.
|429          | **tooManyRequests**       | O aplicativo ou o usuário foi restringido.
|500          | **internalServerError**   | Ocorreu um erro interno do servidor durante o processamento da solicitação.
|501          | **Notimplemented**        | O recurso solicitado não foi implementado.
|502          | **badGateway**            | O servidor encontrou um erro temporário e não pôde concluir sua solicitação.
|503          | **serviceUnavailable**    | O serviço não está disponível. Tente sua solicitação novamente.
|504          | **gatewayTimeout**        | O servidor, enquanto atua como um proxy, não recebeu uma resposta em tempo hábil do servidor upstream para concluir a solicitação.

## <a name="detailed-error-codes"></a>Códigos de erro detalhados

A seguir estão alguns códigos de erro adicionais que seu aplicativo pode encontrar no primeiro nível de objetos aninhados `innerError` . O serviço pode adicionar novos códigos de erro a qualquer momento.

- accessConflict
- Accessdenied
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

> [!NOTE]
> O **objeto innerError** pode conter recursivamente objetos **innerError** mais profundos com códigos de erro adicionais e mais específicos. Esses códigos **innerError** mais profundos destinam-se ao desenvolvedor para ler.

<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->

## <a name="see-also"></a>Confira também

- [Usar a API REST do Excel](/graph/api/resources/excel)