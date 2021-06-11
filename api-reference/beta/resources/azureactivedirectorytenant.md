---
title: Tipo de recurso do azureActiveDirectoryTenant
description: O tipo azureActiveDirectoryTenant identifica outro locatário Azure Active Directory como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d7a36c8c737866b20585518e1dc34e6944c97885
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896582"
---
# <a name="azureactivedirectorytenant-resource-type"></a>Tipo de recurso do azureActiveDirectoryTenant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md). O valor indica que esse tipo identifica outro locatário Azure Active Directory como uma fonte de `@odata.type` identidade para uma organização `#microsoft.graph.azureActiveDirectoryTenant` conectada.

Ao criar uma nova [connectedOrganization](../api/connectedorganization-post.md), se o chamador fornece na coleção identitySources um domainIdentitySource e o domínio corresponde a um domínio registrado de um locatário do Azure Active Directory, a organização conectada resultante criada terá uma coleção identitySources contendo um único membro do tipo [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| displayName |Cadeia de caracteres | O nome do Azure Active Directory locatário. Somente leitura. |
| tenantId |String | A ID do Azure Active Directory locatário. Somente leitura. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "azureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


