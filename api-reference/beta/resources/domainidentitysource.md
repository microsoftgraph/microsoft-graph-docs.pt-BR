---
title: Tipo de recurso domainIdentitySource
description: O tipo domainIdentitySource identifica um domínio não locatário como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ae616c98b2ca20ec4e5d9c7aceeba5bdeb538e81
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759661"
---
# <a name="domainidentitysource-resource-type"></a>Tipo de recurso domainIdentitySource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md). O `@odata.type` valor indica que esse tipo identifica um domínio como uma fonte de identidade para uma organização `#microsoft.graph.domainIdentitySource` conectada.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| displayName |Cadeia de caracteres | O nome da fonte de identidade, normalmente também o nome de domínio. Somente leitura. |
| domainName |Cadeia de caracteres | O nome de domínio. Somente leitura. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


