---
title: tipo de recurso sharingDetail
description: 'Tipo complexo contendo propriedades de itens compartilhados. '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4a2dc75ed2a62d7a67538bdef801bd97133fbd15
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333558"
---
# <a name="sharingdetail-resource-type"></a>tipo de recurso sharingDetail

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipo complexo contendo propriedades de itens [compartilhados](insights-shared.md) . 

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
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo          | Descrição  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| A data e a hora em que o arquivo foi compartilhado pela última vez. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`. Somente leitura.  |
| sharingSubject        | String          | O assunto com o qual o documento foi compartilhado. |
| sharingtype             | String        | Determina o modo como o documento foi compartilhado, pode ser um "link", "anexo", "grupo", "site".     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | O usuário que compartilhou o documento.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |
