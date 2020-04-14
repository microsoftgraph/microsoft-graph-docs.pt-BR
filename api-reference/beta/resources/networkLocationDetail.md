---
title: tipo de recurso networkLocationDetail
description: Fornece o nome e o tipo de rede a partir da qual o usuário entrou.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 88146920f769afbc833d53bb9455ee046f5961e3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459780"
---
# <a name="networklocationdetail-resource-type"></a>tipo de recurso networkLocationDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece o nome e o tipo de rede a partir da qual o usuário entrou.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|networknames|Coleção de cadeias de caracteres|Fornece o nome da rede usada ao entrar.|
|NetworkType|NetworkType| Fornece o tipo de rede usada ao entrar. Os valores possíveis são: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail",
  "baseType": null
}-->

```json
{
  "networkNames": ["String"],
  "networkType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->