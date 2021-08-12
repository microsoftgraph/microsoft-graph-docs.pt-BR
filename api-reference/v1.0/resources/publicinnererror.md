---
title: Tipo de recurso publicInnerError
description: Representa os detalhes internos de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e9e3bbc643666d3dc0596915e8734802065bca413f6d5d73bc51d880a64d1b5c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178000"
---
# <a name="publicinnererror-resource-type"></a>Tipo de recurso publicInnerError

Namespace: microsoft.graph

Representa os detalhes internos de [um publicError](../resources/publicerrordetail.md). 
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|Cadeia de caracteres|O código de erro.|
|detalhes|[Coleção publicErrorDetail](../resources/publicerrordetail.md)|Uma coleção de detalhes de erro.|
|mensagem|String|A mensagem de erro.|
|destino|Cadeia de caracteres|O destino do erro.|

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
