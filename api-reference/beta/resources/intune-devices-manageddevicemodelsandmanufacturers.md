---
title: tipo de recurso managedDeviceModelsAndManufacturers
description: Modela e fabrica meatadata para dispositivos gerenciados na conta
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7cfedad0fce093d8fc3358afcf622ac8beb58d6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999771"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>tipo de recurso managedDeviceModelsAndManufacturers

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modela e fabrica meatadata para dispositivos gerenciados na conta

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceModels|Coleção de cadeias de caracteres|Lista de modelos para dispositivos gerenciados na conta|
|deviceManufacturers|Coleção de cadeias de caracteres|Lista de fabricantes de dispositivos gerenciados na conta|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```





