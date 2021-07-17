---
title: Tipo de recurso publicErrorDetail
description: Representa os detalhes de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac86f2aa50e1447702099f3c73f31979b6e6eb16
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467235"
---
# <a name="publicerrordetail-resource-type"></a>Tipo de recurso publicErrorDetail

Namespace: microsoft.graph

Representa os detalhes [de publicError](../resources/publicerror.md) ou [publicInnerError](../resources/publicinnererror.md).

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
