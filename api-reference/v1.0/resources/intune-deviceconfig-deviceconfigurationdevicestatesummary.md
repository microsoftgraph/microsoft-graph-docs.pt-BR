---
title: Tipo de recurso deviceConfigurationDeviceStateSummary
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e948c064afe4afefa0e2c8685a3654491c8c4513
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573365"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a>Tipo de recurso deviceConfigurationDeviceStateSummary

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceConfigurationDeviceStateSummary](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Ler propriedades e relações de objetos de [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).|
|[Atualizar deviceConfigurationDeviceStateSummary](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Atualizar as propriedades do objeto de [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|unknownDeviceCount|Int32|Número de dispositivos desconhecidos|
|notApplicableDeviceCount|Int32|Número de dispositivos não aplicáveis|
|compliantDeviceCount|Int32|Número de dispositivos em conformidade|
|remediatedDeviceCount|Int32|Número de dispositivos corrigidos|
|nonCompliantDeviceCount|Int32|Número de dispositivos sem conformidade|
|errorDeviceCount|Int32|Número de dispositivos com erro|
|conflictDeviceCount|Int32|Número de dispositivos em conflito|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



