---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
ms.openlocfilehash: be873ba2b5f9bc1fdd387407c1036435dc6f1fc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036260"
---
# <a name="mentionaction-resource-type"></a>Tipo de recurso MentionAction

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.

[atividade]: itemactivity.md

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

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo                       | Descrição
|:--------------|:---------------------------|:-----------------------------
| mentionees    | Coleção [identitySet][] | As identidades dos usuários mencionados nesta ação.

[identitySet]: identityset.md

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
