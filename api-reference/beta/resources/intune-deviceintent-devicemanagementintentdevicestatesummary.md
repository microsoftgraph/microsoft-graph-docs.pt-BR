---
title: tipo de recurso deviceManagementIntentDeviceStateSummary
description: Entidade que representa o resumo de estado do dispositivo para uma intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b87b37a61f3847f77e38fd429c9dd7096235cfff
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708799"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a>tipo de recurso deviceManagementIntentDeviceStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o resumo de estado do dispositivo para uma intenção

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementIntentDeviceStateSummary](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .|
|[Atualizar deviceManagementIntentDeviceStateSummary](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Atualiza as propriedades de um objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID|
|conflictCount|Int32|Número de dispositivos em conflito|
|errorCount|Int32|Número de dispositivos com erro|
|failedCount|Int32|Número de dispositivos com falha|
|notApplicableCount|Int32|Número de dispositivos não aplicáveis|
|notApplicablePlatformCount|Int32|Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis|
|successCount|Int32|Número de dispositivos com êxito|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024
}
```





