---
title: insightIdentity
description: Tipo complexo que contém propriedades de itens compartilhados.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 701840cea5f1bc5e878e5d47c21caf97aed320de
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129862"
---
# <a name="insightidentity"></a>insightIdentity

Namespace: microsoft.graph

Tipo complexo que contém propriedades de [itens sharedInsight.](insights-shared.md) 

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
| id              | Cadeia de caracteres        | A id do usuário que compartilhou o item.     |
| address             | Cadeia de caracteres      | O endereço de email do usuário que compartilhou o item.  |

