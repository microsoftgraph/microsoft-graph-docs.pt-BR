---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8718ab248dada75f04d92d6a8717dd4f43ee8106
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333593"
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
