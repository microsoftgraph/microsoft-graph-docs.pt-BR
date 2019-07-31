---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 6b5a4b3c6e43f0314860935af810d20d91663c96
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005748"
---
# <a name="insightidentity"></a>insightIdentity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipo complexo contendo propriedades de itens [compartilhados](insights-shared.md) . 

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
| displayName       | String          | O nome de exibição do usuário que compartilhou o item. |
| id              | String        | A ID do usuário que compartilhou o item.     |
| address             | Cadeia de caracteres      | O endereço de email do usuário que compartilhou o item.  |
