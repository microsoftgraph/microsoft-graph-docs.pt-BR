---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3a23344a18979c7d1aa69b8e841007812797b238
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531298"
---
# <a name="insightidentity"></a>insightIdentity

Namespace: microsoft.graph

Tipo complexo contendo propriedades de itens do [sharedInsight](insights-shared.md) . 

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo          | Descrição  |
| -------------         |-----------    | -------------|
| displayName       | Cadeia de caracteres          | O nome de exibição do usuário que compartilhou o item. |
| id              | String        | A ID do usuário que compartilhou o item.     |
| address             | Cadeia de caracteres      | O endereço de email do usuário que compartilhou o item.  |
