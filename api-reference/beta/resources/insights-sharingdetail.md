---
title: Tipo de recurso sharingDetail
description: 'Tipo complexo que contém propriedades de itens compartilhados. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c34d0bf2d35f51ecae7268ef754a228dc226664a
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473889"
---
# <a name="sharingdetail-resource-type"></a>Tipo de recurso sharingDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| sharingSubject        | String          | O assunto com o qual o documento foi compartilhado. |
| sharingType             | String        | Determina como o documento foi compartilhado, pode ser por um "Link", "Attachment", "Group", "Site".     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | O usuário que compartilhou o documento.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |


