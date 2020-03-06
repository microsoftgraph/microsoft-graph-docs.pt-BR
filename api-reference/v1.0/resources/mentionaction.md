---
author: daspek
ms.author: dspektor
title: tipo de recurso mençãoaction
description: O objeto Mençãoaction fornece informações sobre quem foi mencionado durante uma atividade.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: de6bf1657e9b9ba21d589a6ef27292553bf93f7e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534244"
---
# <a name="mentionaction-resource-type"></a>tipo de recurso mençãoaction

Namespace: microsoft.graph

O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

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
