---
title: Tipo de recurso monitoringSettings
description: Configurações controlar o monitoramento automatizado e a resposta em uma implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: aff5fa9571628783521dcc5ae0113e767915c2c7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067792"
---
# <a name="monitoringsettings-resource-type"></a>Tipo de recurso monitoringSettings

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações controlar o monitoramento automatizado e a resposta em uma implantação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|monitoringRules|[coleção microsoft.graph.windowsUpdates.monitoringRule](../resources/windowsupdates-monitoringrule.md)|Especifica as regras pelas quais os sinais de monitoramento podem disparar ações na implantação. As regras são combinadas usando "ou".|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringSettings",
  "monitoringRules": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
    }
  ]
}
```

