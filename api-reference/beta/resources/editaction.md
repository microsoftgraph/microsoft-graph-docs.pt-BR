---
author: daspek
description: A presença do recurso EditAction em uma itemActivity indica que a atividade editou um item.
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 374b4f7374ba91360bdaa97e5bc36fb0f5aabbae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006504"
---
# <a name="editaction-resource-type"></a>Tipo de recurso EditAction

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
