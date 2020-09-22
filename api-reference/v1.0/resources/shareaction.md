---
author: daspek
ms.author: dspektor
title: tipo de recurso shareaction
description: O objeto shareaction fornece informações sobre quem um item foi compartilhado em uma ação de compartilhamento.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 90d1d05a16130109dcef200938640e88e63e393a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009202"
---
# <a name="shareaction-resource-type"></a>tipo de recurso shareaction

Namespace: microsoft.graph

O recurso **shareaction** fornece informações sobre uma [atividade][activity] que compartilhou um item.

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

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
  "@type": "microsoft.graph.shareAction"
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

