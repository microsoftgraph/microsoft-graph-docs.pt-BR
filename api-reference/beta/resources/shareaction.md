---
author: daspek
description: O recurso ShareAction fornece informações sobre uma activity que compartilhou um item.
ms.date: 09/14/2017
title: ShareAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: b8cccedfe4d71f7a490d303201f56cec22fd4051
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731579"
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
