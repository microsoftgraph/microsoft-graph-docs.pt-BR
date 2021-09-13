---
title: Tipo de recurso publicInnerError
description: Representa os detalhes internos de um erro.
author: AkJo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2c0189ee65de82edc87f1c9637351409241c00ca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143815"
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
