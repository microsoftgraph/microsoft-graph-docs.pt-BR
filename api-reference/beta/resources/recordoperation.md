---
title: tipo de recurso de recordOperation
description: O tipo de recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: be6a124fcd7175489679a8c2392218530d510e9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880014"
---
# <a name="recordoperation-resource-type"></a>tipo de recurso de recordOperation

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O tipo de recordOperation

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                        | Descrição                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | Cadeia de caracteres                      | O contexto de cliente.                                                                                                                               |
| completionReason               | Cadeia de caracteres                      | Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`. |
| createdDateTime                | DateTimeOffset              | A hora em que a gravação foi criada.                                                                                                          |
| id                             | Cadeia de caracteres                      | A identificação de operação do servidor. Somente leitura. Servidor foi gerado.                                                                                             |
| lastActionDateTime             | DateTimeOffset              | A hora da última ação da operação.                                                                                                     |
| recordResourceAccessToken      | Cadeia de caracteres                      | O token de acesso necessário para recuperar a gravação.                                                                                              |
| recordResourceLocation         | Cadeia de caracteres                      | O local onde a gravação está localizada.                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | As informações de resultado.  Somente leitura. Servidor foi gerado.                                                                                             |
| status                         | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura. Servidor foi gerado.                                                 |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>Exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
