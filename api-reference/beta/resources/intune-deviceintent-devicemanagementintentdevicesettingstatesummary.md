---
title: tipo de recurso deviceManagementIntentDeviceSettingStateSummary
description: Entidade que representa o resumo de estado de configuração de dispositivo para uma intenção
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3c3e6a3630d3e28e62555db25565ab916dc7a91
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524054"
---
# <a name="devicemanagementintentdevicesettingstatesummary-resource-type"></a>tipo de recurso deviceManagementIntentDeviceSettingStateSummary

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o resumo de estado de configuração de dispositivo para uma intenção

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntentDeviceSettingStateSummaries](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-list.md)|coleção [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Listar Propriedades e relações dos objetos [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|
|[Obter deviceManagementIntentDeviceSettingStateSummary](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-get.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|
|[Criar deviceManagementIntentDeviceSettingStateSummary](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-create.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Criar um novo objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|
|[Excluir deviceManagementIntentDeviceSettingStateSummary](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-delete.md)|Nenhum|Exclui [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).|
|[Atualizar deviceManagementIntentDeviceSettingStateSummary](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-update.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Atualiza as propriedades de um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID|
|settingName|Cadeia de caracteres|Nome de uma configuração|
|compliantCount|Int32|Número de dispositivos em conformidade|
|conflictCount|Int32|Número de dispositivos em conflito|
|errorCount|Int32|Número de dispositivos com erro|
|nonCompliantCount|Int32|Número de dispositivos não compatíveis|
|notApplicableCount|Int32|Número de dispositivos não aplicáveis|
|remediatedCount|Int32|Número de dispositivos corrigidos|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceSettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "compliantCount": 1024,
  "conflictCount": 1024,
  "errorCount": 1024,
  "nonCompliantCount": 1024,
  "notApplicableCount": 1024,
  "remediatedCount": 1024
}
```







