---
author: daspek
title: Tipo de recurso mentionAction
description: O objeto MentionAction fornece informações sobre quem foi mencionado durante uma atividade.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: bdcef79492604aa5ee2afae0897361eb41dd6889229b4b41259cc3d47f72bf92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152380"
---
# <a name="mentionaction-resource-type"></a>Tipo de recurso mentionAction

Namespace: microsoft.graph

O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.

>**Observação:** No momento, os registros de atividade do item estão disponíveis apenas SharePoint e OneDrive for Business.

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
  "@type&quot;: &quot;microsoft.graph.mentionAction"
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

