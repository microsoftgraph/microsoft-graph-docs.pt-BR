---
author: daspek
description: A presença do recurso CreateAction em uma itemActivity indica que a atividade criou um item.
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 349a46b4fc4b13fd597f120fdc4ca4d6641e932e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507363"
---
# <a name="createaction-resource-type"></a>Tipo de recurso CreateAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **CreateAction** em uma [**itemActivity**][activity] indica que a atividade criou um item.

**Observação**: embora esse recurso esteja vazio no momento, em revisões futuras da API ele poderá ser preenchido com propriedades adicionais.

[activity]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
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
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction",
  "suppressions": []
}
-->
