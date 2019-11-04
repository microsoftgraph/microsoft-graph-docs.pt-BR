---
title: tipo de recurso de Multiface
description: tipo de recurso de Multiface
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: bb89037b3d5b88e57ec12b2b02a5e2ed37cb2601
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939324"
---
# <a name="itemfacet-resource-type"></a>tipo de recurso de Multiface

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o tipo de base abstrato que todos os tipos de recurso no EntitySet de [perfil](profile.md) herdam de.

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                            | Descrição |
|:---------------------|:--------------------------------|:------------|
|allowedAudiences      |string                           | Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.  |
|createdBy             |[identitySet](identityset.md)    | Quando a entidade foi originalmente criada.   |
|createdDateTime       |DateTimeOffset                   |O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id                    |String                           | Somente leitura.|
|fracassa             |[inferenceData](inferencedata.md)| Contém detalhes de inferência se a entidade for inferida. |
|lastModifiedBy        |[identitySet](identityset.md)    | Identificador do parceiro ou usuário que modificou a entidade pela última vez. |
|lastModifiedDateTime  |DateTimeOffset                   |O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "allowedAudiences": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "inference": {"@odata.type": "microsoft.graph.inferenceData"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemFacet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->