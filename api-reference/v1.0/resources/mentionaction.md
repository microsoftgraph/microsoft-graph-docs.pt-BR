---
author: daspek
title: Tipo de recurso mentionAction
description: O objeto MentionAction fornece informações sobre quem foi mencionado durante uma atividade.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: bc876f05949beb09b3e495a8b9b0536070b352cb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238383"
---
# <a name="mentionaction-resource-type"></a>Tipo de recurso mentionAction

Namespace: microsoft.graph

O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.

>**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.

[atividade]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo                       | Descrição
|:--------------|:---------------------------|:-----------------------------
| mentionees    | Coleção [identitySet][] | As identidades dos usuários mencionados nesta ação.

[identitySet]: identityset.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

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

