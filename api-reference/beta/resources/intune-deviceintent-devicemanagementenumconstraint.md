---
title: Tipo de recurso deviceManagementEnumConstraint
description: A restrição que impõe o valor de configuração é de um conjunto permitido de cadeias de caracteres
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 663ddf69f7b46b9029f5d5ff0b83ee6b84ccd9b6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785133"
---
# <a name="devicemanagementenumconstraint-resource-type"></a>Tipo de recurso deviceManagementEnumConstraint

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A restrição que impõe o valor de configuração é de um conjunto permitido de cadeias de caracteres


Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|values|[Coleção deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md)|Lista de valores válidos para essa cadeia de caracteres|

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



