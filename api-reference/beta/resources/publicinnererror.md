---
title: Tipo de recurso publicInnerError
description: Representa os detalhes internos de um erro.
author: AkJo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dc618025e32e57f91802a6a6101529190474d148
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59050968"
---
# <a name="publicinnererror-resource-type"></a>Tipo de recurso publicInnerError

Namespace: microsoft.graph

Representa os detalhes internos de [um publicError](../resources/publicerrordetail.md). 
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|Cadeia de Caracteres|O código de erro.|
|detalhes|[Coleção publicErrorDetail](../resources/publicerrordetail.md)|Uma coleção de detalhes de erro.|
|mensagem|String|A mensagem de erro.|
|destino|Cadeia de Caracteres|O destino do erro.|

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

