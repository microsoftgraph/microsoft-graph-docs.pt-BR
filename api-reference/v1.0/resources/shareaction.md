---
author: daspek
title: Tipo de recurso shareAction
description: O objeto shareAction fornece informações sobre a quem um item foi compartilhado em uma ação de compartilhamento.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b9d252df884e90d7351edb9544a354d88fbc78baebcc5926686b016c38e58f37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251775"
---
# <a name="shareaction-resource-type"></a>Tipo de recurso shareAction

Namespace: microsoft.graph

O **recurso shareAction** fornece informações sobre uma [atividade][activity] que compartilhou um item.

>**Observação:** No momento, os registros de atividade do item estão disponíveis apenas SharePoint e OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo                       | Descrição
|:--------------|:---------------------------|:-----------------------------
| destinatários    | Coleção [identitySet][] | As identidades com as quais o item foi compartilhado nesta ação.

[identitySet]: identityset.md

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

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->

