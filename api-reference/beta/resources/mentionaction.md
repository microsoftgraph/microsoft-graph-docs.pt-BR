---
author: daspek
description: O recurso MentionAction fornece informações sobre um atividade que mencionou pessoas.
ms.date: 09/14/2017
title: MentionAction
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4675a732738741dc5bb201f97753dca2be42a17d
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723483"
---
# <a name="mentionaction-resource-type"></a>Tipo de recurso MentionAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.

[atividade]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                       | Descrição                                           |
| :--------- | :------------------------- | :---------------------------------------------------- |
| mentionees | Coleção [identitySet][] | As identidades dos usuários mencionados nesta ação. |

[identitySet]: identityset.md

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": []
}
-->
