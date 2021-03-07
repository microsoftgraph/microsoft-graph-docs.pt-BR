---
title: Tipo de recurso printMargin
description: Especifica as larguras de margem a ser usadas durante a impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1680cc641da02f3339dcd75977c411d3255cf037
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517035"
---
# <a name="printmargin-resource-type"></a>Tipo de recurso printMargin

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

