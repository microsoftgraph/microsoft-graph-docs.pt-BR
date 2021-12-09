---
title: Tipo de recurso cloudPcLoginResult
description: Representa os detalhes dos resultados do Cloud PC.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b0ab1d22d5eabeaed84e8ee0d15f9527d64387e7
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391100"
---
# <a name="cloudpcloginresult-resource-type"></a>Tipo de recurso cloudPcLoginResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes dos resultados do Cloud PC.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hora|DateTimeOffSet|O tempo do cloud pc suspira em ação. O timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como '2014-01-01T00:00:00Z'. Somente leitura.|

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
