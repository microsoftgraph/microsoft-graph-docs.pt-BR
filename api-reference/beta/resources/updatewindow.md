---
title: tipo de recurso updateWindow
description: tipo de recurso updateWindow.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 57fb977dd853261300ed09dd8d9b3c343f62bea0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840951"
---
# <a name="updatewindow-resource-type"></a>tipo de recurso updateWindow

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a janela de tempo durante a qual [os agentes](onpremisesagent.md) podem receber atualizações.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|updateWindowEndTime|TimeOfDay|Término de uma janela de tempo durante a qual os agentes podem receber atualizações|
|updateWindowStartTime|TimeOfDay|Início de uma janela de tempo durante a qual os agentes podem receber atualizações|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateWindow",
  "baseType": null
}-->

```json
{
  "updateWindowEndTime": "String (timestamp)",
  "updateWindowStartTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "updateWindow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
