---
title: Tipo de recurso deviceConfigurationDeviceOverview
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e6ded68974f3a4baa307d186e93ea83931f07aa
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773221"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a>Tipo de recurso deviceConfigurationDeviceOverview

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Acessar deviceConfigurationDeviceOverview](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Leia as propriedades e relações de objetos de [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).|
|[Atualizar deviceConfigurationDeviceOverview](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Atualizar as propriedades de um objeto de [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|pendingCount|Int32|Número de dispositivos pendentes|
|notApplicableCount|Int32|Número de dispositivos não aplicáveis|
|notApplicablePlatformCount|Int32|Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis|
|successCount|Int32|Número de dispositivos com êxito|
|errorCount|Int32|Número de dispositivos com erro|
|failedCount|Int32|Número de dispositivos com falha|
|conflictCount|Int32|Número de dispositivos em conflito|
|lastUpdateDateTime|DateTimeOffset|Hora da última atualização|
|configurationVersion|Int32|Versão da política para essa visão geral|

## <a name="relationships"></a>Relações
Nenhuma

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
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





