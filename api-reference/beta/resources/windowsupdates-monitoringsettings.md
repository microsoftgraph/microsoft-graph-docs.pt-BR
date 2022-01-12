---
title: Tipo de recurso monitoringSettings
description: Configurações controlar o monitoramento automatizado e a resposta em uma implantação.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: c00f7e714b68595ce1debbf155ec802f0f579f23
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61810434"
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

