---
title: Tipo de recurso sharingDetail
description: 'Tipo complexo que contém propriedades de itens compartilhados. '
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 96840e801e7789c287dad26e014797013039a6a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094286"
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
| sharedDateTime        | DateTimeOffset| A data e a hora em que o arquivo foi compartilhado pela última vez. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.  |
| sharingSubject        | String          | O assunto com o qual o documento foi compartilhado. |
| sharingType             | Cadeia de caracteres        | Determina como o documento foi compartilhado, pode ser por um "Link", "Attachment", "Group", "Site".     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | O usuário que compartilhou o documento.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |

