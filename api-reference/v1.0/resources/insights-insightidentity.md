---
title: insightIdentity
description: Tipo complexo que contém propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 393a6c1f7fbd1a7fffac667afcf054cdc6b54d55576ffb220df6437166827622
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229247"
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
| displayName       | Cadeia de caracteres          | O nome de exibição do usuário que compartilhou o item. |
| id              | Cadeia de caracteres        | A id do usuário que compartilhou o item.     |
| address             | Cadeia de caracteres      | O endereço de email do usuário que compartilhou o item.  |

