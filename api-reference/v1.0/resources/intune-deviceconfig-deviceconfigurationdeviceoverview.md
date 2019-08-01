---
title: Tipo de recurso deviceConfigurationDeviceOverview
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25abfce9ad69ea6f658a8883cb227806362a6cff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028438"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a>Tipo de recurso deviceConfigurationDeviceOverview

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceConfigurationDeviceOverview](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Ler propriedades e relações de objetos de [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).|
|[Atualizar deviceConfigurationDeviceOverview](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Atualizar as propriedades de um objeto de [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|pendingCount|Int32|Número de dispositivos pendentes|
|notApplicableCount|Int32|Número de dispositivos não aplicáveis|
|successCount|Int32|Número de dispositivos com êxito|
|errorCount|Int32|Número de dispositivos com erro|
|failedCount|Int32|Número de dispositivos com falha|
|lastUpdateDateTime|DateTimeOffset|Hora da última atualização|
|configurationVersion|Int32|Versão da política para essa visão geral|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



