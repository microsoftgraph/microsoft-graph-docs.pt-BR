---
title: tipo de recurso de configuração
description: Especifica IDs de aplicativo adicionais que têm permissão para gerenciar o externalConnection e indexar o conteúdo em um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7808d014ee2ab19fda9eceb6064375cf5904d52
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704147"
---
# <a name="configuration-resource-type"></a>tipo de recurso de configuração

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica IDs de aplicativo adicionais que têm permissão para gerenciar o externalConnection e indexar o conteúdo em um [externalConnection](../resources/externalconnection.md).

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo              | Descrição |
|:---------------|:------------------|:------------|
| authorizedApps | Coleção de cadeias de caracteres | Uma coleção de IDs de aplicativo para aplicativos registrados do Active Directory do Azure que têm permissão para gerenciar o externalConnection e indexar o conteúdo no externalConnection. |

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
