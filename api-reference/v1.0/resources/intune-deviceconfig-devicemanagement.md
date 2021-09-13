---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b8b4373dbbb4679b70c80bd2661b0a11b8dbfc2c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128281"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-deviceconfig-devicemanagement-get.md)|[deviceManagement](../resources/intune-deviceconfig-devicemanagement.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-deviceconfig-devicemanagement-update.md)|[deviceManagement](../resources/intune-deviceconfig-devicemanagement.md)|Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Configurações de nível da conta.|
|intuneAccountId|Guid|ID da conta do Intune para determinado locatário|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|As configurações de dispositivos.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|As políticas de conformidade do dispositivo.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|O resumo do status de atualização do software.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|O resumo do estado de conformidade dos dispositivos para esta conta.|
|deviceCompliancePolicySettingStateSummaries|Coleção [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Os estados resumidos das configurações da política de conformidade para esta conta.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|O resumo do estado de configuração de dispositivos para esta conta.|
|iosUpdateStatuses|Coleção [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Os status de instalação de atualizações de software do iOS para esta conta.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  },
  "intuneAccountId": "Guid"
}
```




