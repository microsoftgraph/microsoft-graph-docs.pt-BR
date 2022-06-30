---
title: Códigos de erro para APIs de pastas de trabalho e gráficos
description: Lista e descreve os códigos de erro retornados pelas APIs de pastas de trabalho e gráficos no Microsoft Graph quando uma solicitação enviada por meio da API falha.
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: d51b2da336e5d27177f654dfff25c86adcd0dd79
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555853"
---
# <a name="error-codes-for-workbooks-and-charts-apis"></a>Códigos de erro para APIs de pastas de trabalho e gráficos

Este artigo descreve os códigos de erro retornados pelas APIs de pastas de trabalho e gráficos no Microsoft Graph quando uma solicitação enviada por meio dessas APIs falha. Para obter detalhes sobre como lidar com respostas de erro de APIs de pastas de trabalho e gráficos no Microsoft Graph, consulte Tratamento de erros para [APIs do Excel no Microsoft Graph](workbook-error-handling.md). Para obter mais detalhes sobre respostas de erro e tipos de recursos no Microsoft Graph, consulte respostas [de erro e tipos de recursos do Microsoft Graph](errors.md).

## <a name="error-codes-and-messages"></a>Códigos de erro e mensagens

A tabela a seguir lista os códigos de erro e as mensagens atuais. O serviço pode adicionar novos códigos de erro a qualquer momento.

| Código de status | Código do erro            | Mensagem de erro                                                                                                                     |
|:------------|:----------------------|:----------------------------------------------------------------------------------------------------------------------------------|
| 400         | `badRequest`          | A solicitação está incorreta ou foi mal formada.                                                                                            |
| 401         | `unauthorized`        | O chamador não está autenticado.                                                                                                  |
| 403         | `forbidden`           | O chamador não tem permissão para executar a ação.                                                                         |
| 404         | `notFound`            | Não foi possível localizar o recurso.                                                                                                  |
| 405         | `methodNotAllowed`    | O método HTTP na solicitação não é permitido no recurso.                                                                    |
| 409         | `conflict`            | O estado atual está em conflito com o que a solicitação espera.                                                                        |
| 413         | `payloadTooLarge`     | O tamanho da solicitação excede o limite máximo.                                                                                       |
| 429         | `tooManyRequests`     | O aplicativo ou o usuário foi restringido.                                                                                               |
| 500         | `internalServerError` | Ocorreu um erro interno do servidor durante o processamento da solicitação.                                                                   |
| 501         | `notImplemented`      | O recurso solicitado não foi implementado.                                                                                          |
| 502         | `badGateway`          | O servidor encontrou um erro temporário e não pôde concluir sua solicitação.                                                     |
| 503         | `serviceUnavailable`  | O serviço não está disponível. Tente sua solicitação novamente.                                                                      |
| 504         | `gatewayTimeout`      | O servidor, enquanto atua como um proxy, não recebeu uma resposta em tempo hábil do servidor upstream para concluir a solicitação. |

## <a name="detailed-error-codes"></a>Códigos de erro detalhados

A seguir estão os códigos de erro necessários que seu aplicativo pode encontrar dentro do primeiro nível de objetos **innerError** aninhados. O serviço pode adicionar novos códigos de erro a qualquer momento.

- `accessConflict`
- `badRequestUncategorized`
- `conflictUncategorized`
- `forbiddenUncategorized`
- `gatewayTimeoutUncategorized`
- `internalServerErrorUncategorized`
- `invalidSessionAccessConflict`
- `invalidSessionAuthentication`
- `invalidSessionNotFound`
- `invalidSessionReCreatable`
- `invalidSessionRestricted`
- `invalidSessionUnexpected`
- `invalidSessionUnsupportedWorkbook`
- `methodNotAllowedUncategorized`
- `notFoundUncategorized`
- `notImplementedUncategorized`
- `payloadTooLargeUncategorized`
- `serviceUnavailableUncategorized`
- `tooManyRequestsUncategorized`
- `transientFailure`
- `unauthorizedUncategorized`
- `unsupportedWorkbook`

Para obter exemplos de códigos de erro opcionais dentro do primeiro nível de objetos **innerError** aninhados, consulte exemplos opcionais de código de erro [de segundo nível](workbook-error-handling.md#optional-second-level-error-code-examples).

> [!NOTE]
> O **objeto innerError** pode conter recursivamente objetos **innerError** mais profundos com códigos de erro adicionais e mais específicos. Esses códigos **innerError** mais profundos destinam-se apenas para fins de diagnóstico.

<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->

## <a name="see-also"></a>Confira também

- [Usar a API REST do Excel](/graph/api/resources/excel)