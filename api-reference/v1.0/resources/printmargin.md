---
title: Tipo de recurso printMargin
description: Especifica as larguras de margem a ser usadas durante a impressão.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 20ad208efdac2890a45dfbebdcf51ace8e49d061
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60924205"
---
# <a name="printmargin-resource-type"></a>Tipo de recurso printMargin

Namespace: microsoft.graph

Especifica as larguras de margem a ser usadas durante a impressão.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|top|Int32|A margem em mícrons da borda superior.|
|bottom|Int32|A margem em mícrons da borda inferior.|
|Certo|Int32|A margem em mícrons da borda direita.|
|left|Int32|A margem em mícrons da borda esquerda.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printMargin"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printMargin",
  "top": "Integer",
  "bottom": "Integer",
  "right": "Integer",
  "left": "Integer"
}
```

