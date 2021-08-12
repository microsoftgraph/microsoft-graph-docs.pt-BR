---
title: Tipo de recurso sharingDetail
description: 'Tipo complexo que contém propriedades de itens compartilhados. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 341bef801b8ee8a7cfc8b5176f4984251209db9e4aff05de9d983b8e06cb61fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124462"
---
# <a name="sharingdetail-resource-type"></a>Tipo de recurso sharingDetail

Namespace: microsoft.graph

Tipo complexo que contém propriedades de [itens sharedInsight.](insights-shared.md) 

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "sharingReference": "resourceReference"
}
```

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo          | Descrição  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| A data e a hora em que o arquivo foi compartilhado pela última vez. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`. Somente leitura.  |
| sharingSubject        | Cadeia de caracteres          | O assunto com o qual o documento foi compartilhado. |
| sharingType             | Cadeia de caracteres        | Determina como o documento foi compartilhado, pode ser por um "Link", "Attachment", "Group", "Site".     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | O usuário que compartilhou o documento.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |

