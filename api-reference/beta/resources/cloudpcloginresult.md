---
title: Tipo de recurso cloudPcLoginResult
description: Representa os detalhes dos resultados de login do Computador na Nuvem.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: f7b083e679939b5d4d478f09ddba6af76a33ac49
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2021
ms.locfileid: "61403072"
---
# <a name="cloudpcloginresult-resource-type"></a>Tipo de recurso cloudPcLoginResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes dos resultados de login do Computador na Nuvem.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hora|DateTimeOffSet|A hora da ação de login do Computador na Nuvem. O timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como '2014-01-01T00:00:00Z'. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcLoginResult",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcLoginResult",
  "time": "String (timestamp)"
}
```
