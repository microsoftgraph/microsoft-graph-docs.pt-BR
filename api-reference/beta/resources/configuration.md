---
title: tipo de recurso de configuração
description: Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8a82c5e9e4cbd915d5a7e11b9e162bc510628ecf
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366771"
---
# <a name="configuration-resource-type"></a>tipo de recurso de configuração

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em [um externalConnection](../resources/externalconnection.md).

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo              | Descrição |
|:---------------|:------------------|:------------|
| authorizedApps | Coleção de cadeias de caracteres | Uma coleção de IDs de aplicativos para aplicativos Azure Active Directory registrados que podem gerenciar o externalConnection e indexar conteúdo no externalConnection. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.configuration",
  "baseType": null
}-->

```json
{
  "authorizedApps": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "configuration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


