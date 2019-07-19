---
title: tipo de recurso deviceManagementEnumConstraint
description: A restrição que impõe o valor da configuração é de um conjunto de cadeias de caracteres permitido
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64c07f663d034cf6fa758155294730015ca6e3b4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964098"
---
# <a name="devicemanagementenumconstraint-resource-type"></a>tipo de recurso deviceManagementEnumConstraint

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A restrição que impõe o valor da configuração é de um conjunto de cadeias de caracteres permitido


Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|values|coleção [deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md)|Lista de valores válidos para esta cadeia de caracteres|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumConstraint",
  "values": [
    {
      "@odata.type": "microsoft.graph.deviceManagementEnumValue",
      "value": "String",
      "displayName": "String"
    }
  ]
}
```





