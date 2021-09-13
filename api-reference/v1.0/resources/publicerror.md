---
title: Tipo de recurso publicError
description: Representa um erro genérico e seus detalhes.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: 4aa4f336ab2b5404e2e82d26f7c38a9ed9b239d2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044290"
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
