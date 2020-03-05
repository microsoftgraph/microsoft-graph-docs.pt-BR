---
title: tipo de recurso provisioningServicePrincipal
description: Representa a entidade de serviço usada para provisionamento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fde8f4d41c7e2788c306fe0e0591b9ddb8ba031d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521331"
---
# <a name="provisioningserviceprincipal-resource-type"></a>tipo de recurso provisioningServicePrincipal

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a entidade de serviço usada para provisionamento. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|Identifica exclusivamente o **servicePrincipalName** usado para provisionamento.|
|nome|String| Nome definido pelo cliente para o **servicePrincipalName**.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningServicePrincipal",
  "baseType": null
}-->

```json
{
  "id": "String",
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
