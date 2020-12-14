---
title: tipo de recurso publicErrorDetail
description: Representa os detalhes de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8620d19d1cd540f7ed523a392e71c304cbbf1774
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659398"
---
# <a name="publicerrordetail-resource-type"></a>tipo de recurso publicErrorDetail

Namespace: microsoft.graph

Representa os detalhes de [publicError](../resources/publicerror.md) ou [publicInnerError](../resources/publicinnererror.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|String|O código de erro.|
|mensagem|String|A mensagem de erro.|
|destino|String|O destino do erro.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorDetail",
  "code": "String",
  "message": "String",
  "target": "String"
}
```

