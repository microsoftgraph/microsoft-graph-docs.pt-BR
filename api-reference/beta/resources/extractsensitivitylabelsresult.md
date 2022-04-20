---
title: Tipo de recurso extractSensitivityLabelsResult
description: Representa o formato de resposta para a API extractSensitivityLabels.
author: jaLuthra
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a3533cecf651c6b98deb81b01cf06d5a08f2dc36
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917806"
---
# <a name="extractsensitivitylabelsresult-resource-type"></a>Tipo de recurso extractSensitivityLabelsResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o formato de resposta para a API [extractSensitivityLabels](../api/driveitem-extractsensitivitylabels.md) .

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Rótulos|[coleção sensitivityLabelAssignment](./sensitivitylabelassignment.md)|Lista de rótulos de confidencialidade atribuídos a um arquivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extractSensitivityLabelsResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extractSensitivityLabelsResult",
  "labels": [
    {
      "@odata.type": "microsoft.graph.sensitivityLabelAssignment"
    }
  ]
}
```

