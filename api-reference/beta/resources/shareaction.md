---
author: daspek
description: O recurso ShareAction fornece informações sobre uma activity que compartilhou um item.
ms.date: 09/14/2017
title: ShareAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 1fba7d65c03981f5336531e37e47731b21e219c0
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722478"
---
# <a name="shareaction-resource-type"></a>Tipo de recurso ShareAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **ShareAction** fornece informações sobre uma [activity][activity] que compartilhou um item.

[activity]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                       | Descrição                                             |
| :--------- | :------------------------- | :------------------------------------------------------ |
| destinatários | Coleção [identitySet][] | As identidades com as quais o item foi compartilhado nesta ação. |

[identitySet]: identityset.md

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": []
}
-->
