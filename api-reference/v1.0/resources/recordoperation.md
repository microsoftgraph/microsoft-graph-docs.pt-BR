---
title: Tipo de recurso recordOperation
description: Esse tipo de recurso contém informações relacionadas à gravação de áudio.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3611eb65f879ab6b70dbe65d9fb1769da6e5dd11
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094097"
---
# <a name="recordoperation-resource-type"></a>Tipo de recurso recordOperation

Namespace: microsoft.graph

Esse tipo de recurso contém informações relacionadas à gravação de áudio.

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                        | Descrição                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | Cadeia de caracteres de contexto de cliente exclusiva. O limite máximo é 256 caracteres.                                                                                                                               |
| id                             | Cadeia de caracteres                      | A id da operação do servidor. Somente leitura.                                                                                              |
| recordingAccessToken           | String                      | O token de acesso necessário para recuperar a gravação.                                                                                              |
| recordingLocation              | Cadeia de caracteres                      | O local onde a gravação está localizada.                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | As informações de resultado.  Somente leitura.                                                                                              |
| status                         | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura.                                                |

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
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

