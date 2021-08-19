---
title: Tipo de recurso managedDeviceModelsAndManufacturers
description: Modelos e Manufaturas de carmadata para dispositivos gerenciados na conta
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d57976ef6d66205a79f60b242ccefc3f8b5bcb20f46ace5be2ab856dc193fd4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249920"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>Tipo de recurso managedDeviceModelsAndManufacturers

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelos e Manufaturas de carmadata para dispositivos gerenciados na conta

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceModels|String collection|Lista de modelos para dispositivos gerenciados na conta|
|deviceManufacturers|String collection|Lista de Manufaturas para dispositivos gerenciados na conta|

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




