---
title: tipo de recurso deviceManagementEnumConstraint
description: A restrição que impõe o valor da configuração é de um conjunto de cadeias de caracteres permitido
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 816782953493bd5c9c790bc3a8785b758cd92137
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275948"
---
# <a name="devicemanagementenumconstraint-resource-type"></a>tipo de recurso deviceManagementEnumConstraint

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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




