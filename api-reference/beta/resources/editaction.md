---
author: daspek
description: A presença do recurso EditAction em uma itemActivity indica que a atividade editou um item.
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 1b7ab5e77b62d3f02ee04a5927cb2294f5c3b5a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502848"
---
# <a name="editaction-resource-type"></a>Tipo de recurso EditAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **EditAction** em uma [**itemActivity**][activity] indica que a atividade editou um item.

**Observação**: embora esse recurso esteja vazio no momento, em revisões futuras da API ele poderá ser preenchido com propriedades adicionais.

[activity]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a>Propriedades

Nenhum. Esta faceta tem um valor nulo ou não nulo e não contém propriedades.

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!--
{
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction",
  "suppressions": []
}
-->
