---
author: daspek
description: O recurso ShareAction fornece informações sobre uma activity que compartilhou um item.
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 94bf1b519308043f3421dc211eac006cfc4fd601
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520742"
---
# <a name="shareaction-resource-type"></a>Tipo de recurso ShareAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **ShareAction** fornece informações sobre uma [activity][activity] que compartilhou um item.

[activity]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo                       | Descrição
|:--------------|:---------------------------|:-----------------------------
| destinatários    | Coleção [identitySet][] | As identidades com as quais o item foi compartilhado nesta ação.

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
