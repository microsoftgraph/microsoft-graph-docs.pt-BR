---
title: tipo de recurso deliveryOptimizationGroupIdSourceOptions
description: Tipo de opções de ID de grupo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d54a98bef3b9c0e0517b426332b8d3223e904c8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177851"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a>tipo de recurso deliveryOptimizationGroupIdSourceOptions

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de opções de ID de grupo


Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|groupIdSourceOption|[deliveryOptimizationGroupIdOptionsType](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|Defina essa política para restringir a seleção de par para uma fonte específica. Os valores possíveis são: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSourceOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdSourceOptions",
  "groupIdSourceOption": "String"
}
```




