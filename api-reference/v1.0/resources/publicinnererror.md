---
title: Tipo de recurso publicInnerError
description: Representa os detalhes internos de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f089c120ac4ba1307f0b0ffa2f08f8578613eaa1
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467234"
---
# <a name="publicinnererror-resource-type"></a>Tipo de recurso publicInnerError

Namespace: microsoft.graph

Representa os detalhes internos de [um publicError](../resources/publicerrordetail.md). 
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|String|O código de erro.|
|detalhes|[Coleção publicErrorDetail](../resources/publicerrordetail.md)|Uma coleção de detalhes de erro.|
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
