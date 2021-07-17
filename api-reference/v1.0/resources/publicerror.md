---
title: Tipo de recurso publicError
description: Representa um erro genérico e seus detalhes.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: e9f5decf8edc2ebf3e11d00eb89e68236a6a73d4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467237"
---
# <a name="publicerror-resource-type"></a>Tipo de recurso publicError

Namespace: microsoft.graph

Representa um erro genérico e seus detalhes.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|cadeia de caracteres| Representa o código de erro.
|detalhes|[Coleção publicErrorDetail](publicerrordetail.md)|Detalhes do erro.|
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
