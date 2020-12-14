---
title: tipo de recurso publicInnerError
description: Representa os detalhes internos de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e8380e8836076687a2d6ab3e8a0a4a53b8bd6964
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658322"
---
# <a name="publicinnererror-resource-type"></a>tipo de recurso publicInnerError

Namespace: microsoft.graph

Representa os detalhes internos de um [publicError](../resources/publicerrordetail.md). 
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|String|O código de erro.|
|detalhes|coleção [publicErrorDetail](../resources/publicerrordetail.md)|Uma coleção de detalhes de erro.|
|mensagem|String|A mensagem de erro.|
|destino|String|O destino do erro.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicInnerError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicInnerError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ]
}
```

