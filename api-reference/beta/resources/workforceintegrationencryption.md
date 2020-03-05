---
title: tipo de recurso workforceIntegrationEncryption
description: Uma entidade de criptografia que define o protocolo e o segredo para uma integração de força de funcionários.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2d24371a0a999069d80a9ad86afd48ac9e68d38
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519075"
---
# <a name="workforceintegrationencryption-resource-type"></a>tipo de recurso workforceIntegrationEncryption

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma entidade de criptografia que define o protocolo e o segredo de um [workforceintegration](../resources/workforceintegration.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|RDP|String| Os valores possíveis são: `sharedSecret` e `unknownFutureValue`.|
|sigilo|String|Segredo compartilhado de criptografia.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
  "baseType": null
}-->

```json
{
  "protocol": "String",
  "secret": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegrationEncryption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
