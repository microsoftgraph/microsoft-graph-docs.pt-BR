---
title: tipo de recurso publicError
description: Representa um erro genérico e seus detalhes.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: 65a75b6eb2756b92f9da6386390fae3b254f818b
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660083"
---
# <a name="publicerror-resource-type"></a>tipo de recurso publicError

Namespace: microsoft.graph

Representa um erro genérico e seus detalhes.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|cadeia de caracteres| Representa o código de erro.
|detalhes|coleção [publicErrorDetail](publicerrordetail.md)|Detalhes do erro.|
|innerError|[publicInnerError](publicinnererror.md)|Detalhes do erro interno.|
|mensagem|cadeia de caracteres| Uma mensagem não localizada para o desenvolvedor.
|destino|String|O destino do erro.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ],
  "innerError": {
    "@odata.type": "microsoft.graph.publicInnerError"
  }
}
```

