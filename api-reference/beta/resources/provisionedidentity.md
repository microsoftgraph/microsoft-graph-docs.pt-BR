---
title: tipo de recurso provisionedIdentity
description: Descreve a identidade associada ao evento de resumo do objeto de provisionamento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 86363bdf77f83e6903c86362c2797c51d1215073
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521352"
---
# <a name="provisionedidentity-resource-type"></a>tipo de recurso provisionedIdentity

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve a identidade associada ao evento de resumo do objeto de provisionamento. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|detalhes|[detailsInfo](detailsinfo.md)|Detalhes da identidade.|
|displayName|Cadeia de caracteres|Nome para exibição da identidade. |
|id|String|Identifica exclusivamente a identidade.|
|IdentityType|String|Tipo de identidade que foi provisionado, como ' usuário ' ou ' grupo '.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
