---
title: Tipo de recurso externalDomainFederation
description: O tipo externalDomainFederation identifica um domínio não locatário com um provedor de identidade configurado como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: df88fef22c2acb86cadcfaed9a8f5be25da70f9d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760985"
---
# <a name="externaldomainfederation-resource-type"></a>Tipo de recurso externalDomainFederation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md). O valor indica que esse tipo identifica um domínio com um provedor de identidade configurado como uma fonte de `@odata.type` identidade para uma organização `#microsoft.graph.externalDomainFederation` conectada.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| displayName |Cadeia de caracteres | O nome da fonte de identidade, normalmente também o nome de domínio. Somente leitura. |
| domainName |Cadeia de caracteres | O nome de domínio. Somente leitura. |
| issuerUri |Cadeia de Caracteres | O emissorURI da federação de entrada. Somente leitura. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalDomainFederation",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String",
  "issuerUri": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalDomainFederation resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


