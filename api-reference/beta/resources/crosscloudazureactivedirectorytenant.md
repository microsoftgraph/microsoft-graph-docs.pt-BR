---
title: Tipo de recurso crossCloudAzureActiveDirectoryTenant
description: O tipo crossCloudAzureActiveDirectoryTenant identifica outro Azure Active Directory locatário em uma nuvem diferente como uma fonte de identidade para uma organização conectada.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8086a5311626a520b96146205076b04547c0cfce
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694409"
---
# <a name="crosscloudazureactivedirectorytenant-resource-type"></a>Tipo de recurso crossCloudAzureActiveDirectoryTenant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas fontes de identidade de um [objeto connectedOrganization](connectedOrganization.md) . O `@odata.type` valor `#microsoft.graph.crossCloudAzureActiveDirectoryTenant` indica que esse tipo identifica outro locatário Azure AD em uma nuvem diferente como uma fonte de identidade para uma organização conectada.


## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| cloudInstance | String | A ID da nuvem em que o locatário está localizado, um de `microsoftonline.com`, `microsoftonline.us` ou `partner.microsoftonline.cn`. Somente leitura. |
| displayName |Cadeia de caracteres | O nome do locatário Azure Active Directory usuário. Somente leitura. |
| tenantId |String | A ID do locatário do Active Directory do Azure. Somente leitura. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.crossCloudAzureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String",
  "cloudInstance": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "crossCloudAzureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


